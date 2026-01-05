# Signal Processing Mathematical Models: Overdrive, Distortion, Fuzz, Crush

**Document Type:** Tone Theory Research - Mathematical Models
**Version:** 1.0
**Created:** 2026-01-05
**Category:** DSP (Digital Signal Processing) Fundamentals
**Purpose:** Mathematical equations and algorithms for simulating guitar distortion effects

---

## Table of Contents

1. [Mathematical Notation](#mathematical-notation)
2. [Overdrive (Soft Clipping)](#overdrive-soft-clipping)
3. [Distortion (Hard Clipping)](#distortion-hard-clipping)
4. [Fuzz (Square Wave Clipping)](#fuzz-square-wave-clipping)
5. [Crush (Bitcrusher)](#crush-bitcrusher)
6. [Implementation Examples](#implementation-examples)
7. [Parameter Ranges](#parameter-ranges)

---

## Mathematical Notation

**Variables:**
- `x(t)` = Input signal at time t (normalized: -1.0 to +1.0)
- `y(t)` = Output signal at time t
- `g` = Gain factor (amplification before clipping)
- `T` = Threshold (clipping threshold)
- `α` = Smoothness parameter (for soft clipping)
- `n` = Bit depth (for bitcrusher)
- `fs` = Sample rate (for bitcrusher)

**Signal Range:**
- All signals normalized to range [-1.0, +1.0]
- 0 dB = 1.0
- Clipping occurs when |x| > 1.0

---

## Overdrive (Soft Clipping)

### Mathematical Model

Overdrive uses smooth, gradual saturation. Several mathematical functions can model this:

#### 1. Hyperbolic Tangent (tanh) - Most Common

```
y(t) = tanh(g × x(t))
```

**Characteristics:**
- Smooth S-curve saturation
- Asymptotic approach to ±1.0
- Odd-function symmetry (symmetrical clipping)
- Output range: (-1, +1)

**Expanded form:**
```
y(t) = (e^(g×x) - e^(-g×x)) / (e^(g×x) + e^(-g×x))
```

**Gain parameter `g`:**
- `g = 1`: Clean (minimal distortion)
- `g = 2-5`: Light overdrive
- `g = 5-10`: Medium overdrive
- `g = 10-20`: Heavy overdrive

#### 2. Asymmetrical Soft Clipping (Tube Screamer Style)

For asymmetrical clipping (different positive/negative wave treatment):

```
         ⎧  tanh(g₊ × x(t))     if x(t) ≥ 0
y(t) =   ⎨
         ⎩  tanh(g₋ × x(t))     if x(t) < 0
```

Where:
- `g₊` = Gain for positive half
- `g₋` = Gain for negative half
- Typical: `g₊ ≠ g₋` (asymmetrical)

**Example (Tube Screamer):**
- `g₊ = 3.0`
- `g₋ = 5.0`
- Creates even harmonics (richer tone)

#### 3. Cubic Soft Clipping

```
         ⎧  x(t) - (x³(t))/3          if |x(t)| ≤ √3
y(t) =   ⎨
         ⎩  sign(x(t)) × 2√3/3        if |x(t)| > √3
```

**Characteristics:**
- Smooth polynomial clipping
- Less aggressive than tanh
- Vintage tube-like response

#### 4. Arctangent Soft Clipping

```
y(t) = (2/π) × arctan(g × x(t))
```

**Characteristics:**
- Similar to tanh but slightly different curve
- Output range: (-1, +1)
- Smoother transition than tanh

---

## Distortion (Hard Clipping)

### Mathematical Model

Hard clipping abruptly cuts off signal peaks.

#### 1. Simple Hard Clipping

```
         ⎧  +T              if g × x(t) > T
         ⎪
y(t) =   ⎨  g × x(t)        if -T ≤ g × x(t) ≤ T
         ⎪
         ⎩  -T              if g × x(t) < -T
```

Where:
- `T` = Threshold (typically 0.7 to 1.0)
- `g` = Gain (typically 10 to 100)

**Simplified notation:**
```
y(t) = max(-T, min(T, g × x(t)))
```

Or using clamp function:
```
y(t) = clamp(g × x(t), -T, T)
```

#### 2. Asymmetrical Hard Clipping (RAT Style)

```
         ⎧  T₊              if g × x(t) > T₊
         ⎪
y(t) =   ⎨  g × x(t)        if -T₋ ≤ g × x(t) ≤ T₊
         ⎪
         ⎩  -T₋             if g × x(t) < -T₋
```

Where:
- `T₊` = Positive threshold (e.g., 0.7)
- `T₋` = Negative threshold (e.g., 0.5)
- Creates asymmetrical distortion

#### 3. Diode Hard Clipping (with exponential curve)

More accurate diode model:

```
         ⎧  V_f × ln(1 + (g×x(t) - V_f)/I_s)     if x(t) > 0
y(t) =   ⎨
         ⎩  -V_f × ln(1 + (-g×x(t) - V_f)/I_s)   if x(t) ≤ 0
```

Where:
- `V_f` = Forward voltage (typically 0.7V for silicon, 0.3V for germanium)
- `I_s` = Saturation current (typically 10^-12)

**Simplified diode model:**
```
y(t) = V_f × sign(x(t)) × ln(1 + |g × x(t)|/V_f)
```

---

## Fuzz (Square Wave Clipping)

### Mathematical Model

Fuzz creates extreme saturation, approaching square wave.

#### 1. Hard Limiting (Square Wave Approximation)

```
y(t) = sign(g × x(t))
```

Where:
```
         ⎧  +1     if x > 0
sign(x) =⎨   0     if x = 0
         ⎩  -1     if x < 0
```

**Characteristics:**
- Complete saturation
- Pure square wave
- Maximum harmonic distortion
- Too extreme for most uses

#### 2. Soft Square Wave (More Musical)

```
y(t) = tanh(g × x(t))    where g = 50 to 1000
```

**High gain tanh approaches square wave:**
- `g = 50`: Heavy fuzz
- `g = 100`: Extreme fuzz
- `g = 500`: Near square wave

#### 3. Piecewise Fuzz Model

```
         ⎧  +1.0                if g × x(t) > T_high
         ⎪
         ⎪  tanh(k × g × x(t))  if T_low < g × x(t) ≤ T_high
y(t) =   ⎨
         ⎪  tanh(k × g × x(t))  if -T_low ≤ g × x(t) ≤ T_low
         ⎪
         ⎩  -1.0                if g × x(t) < -T_low
```

Where:
- `T_high` = Upper threshold (e.g., 0.3)
- `T_low` = Lower threshold (e.g., 0.1)
- `k` = Smoothness factor (e.g., 5-10)

**Characteristics:**
- Smooth transition into extreme clipping
- More musical than pure square wave
- Models vintage fuzz pedals

#### 4. Germanium Transistor Fuzz Model

```
y(t) = A × (1 - e^(-B × g × x(t)))    for x(t) > 0
y(t) = -A × (1 - e^(B × g × x(t)))    for x(t) ≤ 0
```

Where:
- `A` = Amplitude scaling (typically 1.0)
- `B` = Exponential factor (typically 2-5)
- Models germanium transistor saturation

---

## Crush (Bitcrusher)

### Mathematical Model

Bitcrusher reduces bit depth and/or sample rate.

#### 1. Bit Depth Reduction

```
n_bits = target bit depth (e.g., 8, 4, 2)
n_levels = 2^n_bits

y(t) = round(x(t) × n_levels) / n_levels
```

**Example (8-bit):**
```
n_bits = 8
n_levels = 2^8 = 256

y(t) = round(x(t) × 256) / 256
```

**Effect:**
- Quantizes the signal to discrete levels
- Creates "staircase" waveform
- Lower bits = more distortion

**Bit depth examples:**
- 16-bit: 65,536 levels (CD quality, imperceptible quantization)
- 12-bit: 4,096 levels (subtle grit)
- 8-bit: 256 levels (noticeable lo-fi character)
- 4-bit: 16 levels (extreme digital distortion)
- 2-bit: 4 levels (severe distortion)
- 1-bit: 2 levels (square wave)

#### 2. Sample Rate Reduction

```
fs_target = target sample rate (e.g., 8000 Hz)
fs_original = original sample rate (e.g., 44100 Hz)

downsample_factor = floor(fs_original / fs_target)

y[n] = x[n × downsample_factor]    (sample and hold)
```

**Example (8 kHz from 44.1 kHz):**
```
downsample_factor = floor(44100 / 8000) = 5

Keep every 5th sample, hold value in between
```

**Effect:**
- Creates aliasing artifacts
- Loses high-frequency content
- Lower sample rate = more aliasing

**Sample rate examples:**
- 44.1 kHz: CD quality (no artifacts)
- 22 kHz: Slight high-frequency loss
- 11 kHz: Noticeable aliasing
- 8 kHz: Telephone quality
- 4 kHz: AM radio quality
- 2 kHz: Extreme lo-fi

#### 3. Combined Bit Reduction + Sample Rate Reduction

```
Step 1: Sample rate reduction
  downsample_factor = floor(fs_original / fs_target)
  x_downsampled[n] = x[n × downsample_factor]

Step 2: Bit depth reduction
  n_levels = 2^n_bits
  y[n] = round(x_downsampled[n] × n_levels) / n_levels
```

**Most extreme lo-fi:**
```
n_bits = 4
fs_target = 4000 Hz

Result: 8-bit video game sound
```

#### 4. Dithering (Optional, for smoother sound)

Add small random noise before quantization to reduce harsh artifacts:

```
noise = random(-0.5/n_levels, +0.5/n_levels)
y(t) = round((x(t) + noise) × n_levels) / n_levels
```

**Effect:**
- Trades quantization distortion for gentle noise
- Smoother, less harsh lo-fi sound

---

## Implementation Examples

### Python Implementation

```python
import numpy as np

# ============================================================
# OVERDRIVE (Soft Clipping)
# ============================================================

def overdrive_tanh(x, gain=5.0):
    """
    Soft clipping overdrive using tanh

    Args:
        x: Input signal (numpy array, range -1.0 to +1.0)
        gain: Drive amount (1.0 = clean, 20.0 = heavy)

    Returns:
        y: Output signal (range -1.0 to +1.0)
    """
    return np.tanh(gain * x)


def overdrive_asymmetric(x, gain_pos=3.0, gain_neg=5.0):
    """
    Asymmetrical soft clipping (Tube Screamer style)

    Args:
        x: Input signal
        gain_pos: Gain for positive half cycle
        gain_neg: Gain for negative half cycle

    Returns:
        y: Output signal
    """
    y = np.zeros_like(x)
    y[x >= 0] = np.tanh(gain_pos * x[x >= 0])
    y[x < 0] = np.tanh(gain_neg * x[x < 0])
    return y


def overdrive_cubic(x, gain=2.0):
    """
    Cubic soft clipping

    Args:
        x: Input signal
        gain: Drive amount

    Returns:
        y: Output signal
    """
    x_gained = gain * x
    threshold = np.sqrt(3)

    y = np.zeros_like(x)

    # Below threshold: cubic polynomial
    mask = np.abs(x_gained) <= threshold
    y[mask] = x_gained[mask] - (x_gained[mask]**3) / 3

    # Above threshold: hard limit
    y[x_gained > threshold] = 2 * threshold / 3
    y[x_gained < -threshold] = -2 * threshold / 3

    return y


# ============================================================
# DISTORTION (Hard Clipping)
# ============================================================

def distortion_hard_clip(x, gain=10.0, threshold=0.7):
    """
    Hard clipping distortion

    Args:
        x: Input signal
        gain: Pre-clipping gain
        threshold: Clipping threshold (0.0 to 1.0)

    Returns:
        y: Output signal
    """
    x_gained = gain * x
    return np.clip(x_gained, -threshold, threshold)


def distortion_asymmetric(x, gain=15.0, threshold_pos=0.7, threshold_neg=0.5):
    """
    Asymmetrical hard clipping (RAT style)

    Args:
        x: Input signal
        gain: Pre-clipping gain
        threshold_pos: Positive clipping threshold
        threshold_neg: Negative clipping threshold

    Returns:
        y: Output signal
    """
    x_gained = gain * x
    y = np.clip(x_gained, -threshold_neg, threshold_pos)
    return y


def distortion_diode(x, gain=10.0, vf=0.7, is_param=1e-12):
    """
    Diode-style hard clipping (more accurate model)

    Args:
        x: Input signal
        gain: Pre-clipping gain
        vf: Forward voltage (0.7 for silicon, 0.3 for germanium)
        is_param: Saturation current

    Returns:
        y: Output signal
    """
    x_gained = gain * x

    # Simplified diode equation
    y = vf * np.sign(x_gained) * np.log1p(np.abs(x_gained) / vf)

    return y


# ============================================================
# FUZZ (Square Wave Clipping)
# ============================================================

def fuzz_square_wave(x, gain=100.0):
    """
    Extreme fuzz (square wave approximation)

    Args:
        x: Input signal
        gain: Extremely high gain (50-1000)

    Returns:
        y: Output signal
    """
    return np.tanh(gain * x)


def fuzz_hard_limit(x, gain=50.0):
    """
    Pure square wave fuzz

    Args:
        x: Input signal
        gain: Pre-clipping gain

    Returns:
        y: Output signal (pure ±1.0)
    """
    return np.sign(gain * x)


def fuzz_germanium(x, gain=30.0, A=1.0, B=3.0):
    """
    Germanium transistor fuzz model

    Args:
        x: Input signal
        gain: Pre-saturation gain
        A: Amplitude scaling
        B: Exponential factor

    Returns:
        y: Output signal
    """
    x_gained = gain * x

    y = np.zeros_like(x)
    y[x_gained > 0] = A * (1 - np.exp(-B * x_gained[x_gained > 0]))
    y[x_gained <= 0] = -A * (1 - np.exp(B * x_gained[x_gained <= 0]))

    return y


# ============================================================
# CRUSH (Bitcrusher)
# ============================================================

def bitcrush_depth(x, n_bits=8):
    """
    Bit depth reduction

    Args:
        x: Input signal
        n_bits: Target bit depth (1-16)

    Returns:
        y: Output signal
    """
    n_levels = 2 ** n_bits
    y = np.round(x * n_levels) / n_levels
    return y


def bitcrush_sample_rate(x, original_rate=44100, target_rate=8000):
    """
    Sample rate reduction

    Args:
        x: Input signal (numpy array)
        original_rate: Original sample rate (Hz)
        target_rate: Target sample rate (Hz)

    Returns:
        y: Output signal (same length as input)
    """
    downsample_factor = int(original_rate / target_rate)

    # Sample and hold
    y = np.zeros_like(x)
    for i in range(len(x)):
        sample_index = (i // downsample_factor) * downsample_factor
        y[i] = x[sample_index]

    return y


def bitcrush_full(x, n_bits=8, original_rate=44100, target_rate=8000):
    """
    Combined bit depth + sample rate reduction

    Args:
        x: Input signal
        n_bits: Target bit depth
        original_rate: Original sample rate
        target_rate: Target sample rate

    Returns:
        y: Output signal
    """
    # Step 1: Sample rate reduction
    y = bitcrush_sample_rate(x, original_rate, target_rate)

    # Step 2: Bit depth reduction
    y = bitcrush_depth(y, n_bits)

    return y


def bitcrush_dithered(x, n_bits=8):
    """
    Bit depth reduction with dithering (smoother sound)

    Args:
        x: Input signal
        n_bits: Target bit depth

    Returns:
        y: Output signal
    """
    n_levels = 2 ** n_bits

    # Add dither noise
    dither = np.random.uniform(-0.5/n_levels, 0.5/n_levels, size=x.shape)

    y = np.round((x + dither) * n_levels) / n_levels

    return y


# ============================================================
# EXAMPLE USAGE
# ============================================================

if __name__ == "__main__":
    import matplotlib.pyplot as plt

    # Generate test signal (sine wave)
    sample_rate = 44100
    duration = 0.1  # 100ms
    frequency = 440  # A4

    t = np.linspace(0, duration, int(sample_rate * duration))
    x = np.sin(2 * np.pi * frequency * t)

    # Apply each effect
    y_overdrive = overdrive_tanh(x, gain=5.0)
    y_distortion = distortion_hard_clip(x, gain=10.0)
    y_fuzz = fuzz_square_wave(x, gain=100.0)
    y_crush = bitcrush_full(x, n_bits=4, original_rate=44100, target_rate=8000)

    # Plot results
    fig, axes = plt.subplots(5, 1, figsize=(12, 10))

    axes[0].plot(t, x)
    axes[0].set_title('Original Signal')
    axes[0].set_ylabel('Amplitude')

    axes[1].plot(t, y_overdrive)
    axes[1].set_title('Overdrive (tanh, gain=5)')
    axes[1].set_ylabel('Amplitude')

    axes[2].plot(t, y_distortion)
    axes[2].set_title('Distortion (hard clip, gain=10)')
    axes[2].set_ylabel('Amplitude')

    axes[3].plot(t, y_fuzz)
    axes[3].set_title('Fuzz (tanh, gain=100)')
    axes[3].set_ylabel('Amplitude')

    axes[4].plot(t, y_crush)
    axes[4].set_title('Crush (4-bit, 8kHz)')
    axes[4].set_ylabel('Amplitude')
    axes[4].set_xlabel('Time (s)')

    plt.tight_layout()
    plt.savefig('distortion_comparison.png', dpi=150)
    print("Plot saved as 'distortion_comparison.png'")
```

### C/C++ Implementation (Real-time Audio)

```c
#include <math.h>

// ============================================================
// OVERDRIVE (Soft Clipping)
// ============================================================

float overdrive_tanh(float x, float gain) {
    return tanhf(gain * x);
}

float overdrive_asymmetric(float x, float gain_pos, float gain_neg) {
    if (x >= 0.0f) {
        return tanhf(gain_pos * x);
    } else {
        return tanhf(gain_neg * x);
    }
}

// ============================================================
// DISTORTION (Hard Clipping)
// ============================================================

float distortion_hard_clip(float x, float gain, float threshold) {
    float gained = gain * x;

    if (gained > threshold) return threshold;
    if (gained < -threshold) return -threshold;
    return gained;
}

float distortion_asymmetric(float x, float gain, float thresh_pos, float thresh_neg) {
    float gained = gain * x;

    if (gained > thresh_pos) return thresh_pos;
    if (gained < -thresh_neg) return -thresh_neg;
    return gained;
}

// ============================================================
// FUZZ (Square Wave Clipping)
// ============================================================

float fuzz_square_wave(float x, float gain) {
    return tanhf(gain * x);  // Very high gain
}

float fuzz_hard_limit(float x, float gain) {
    float gained = gain * x;

    if (gained > 0.0f) return 1.0f;
    if (gained < 0.0f) return -1.0f;
    return 0.0f;
}

// ============================================================
// CRUSH (Bitcrusher)
// ============================================================

float bitcrush_depth(float x, int n_bits) {
    int n_levels = 1 << n_bits;  // 2^n_bits
    return roundf(x * n_levels) / n_levels;
}

float bitcrush_sample_rate(float x, int* hold_counter, int downsample_factor, float* held_sample) {
    (*hold_counter)++;

    if (*hold_counter >= downsample_factor) {
        *hold_counter = 0;
        *held_sample = x;
    }

    return *held_sample;
}
```

---

## Parameter Ranges

### Overdrive

| Parameter | Min | Typical | Max | Effect |
|-----------|-----|---------|-----|--------|
| Gain | 1.0 | 5.0 | 20.0 | Clean → Heavy overdrive |
| Threshold | 0.5 | 0.7 | 1.0 | Earlier/later clipping |

**Recommended starting points:**
- Jazz/Clean: `gain = 2.0`
- Blues: `gain = 5.0`
- Rock: `gain = 10.0`

### Distortion

| Parameter | Min | Typical | Max | Effect |
|-----------|-----|---------|-----|--------|
| Gain | 5.0 | 15.0 | 100.0 | Light → Heavy distortion |
| Threshold | 0.3 | 0.7 | 1.0 | Earlier/later clipping |

**Recommended starting points:**
- Crunch: `gain = 10.0, threshold = 0.8`
- Heavy distortion: `gain = 30.0, threshold = 0.5`
- Metal: `gain = 50.0, threshold = 0.3`

### Fuzz

| Parameter | Min | Typical | Max | Effect |
|-----------|-----|---------|-----|--------|
| Gain | 20.0 | 100.0 | 1000.0 | Heavy → Extreme fuzz |

**Recommended starting points:**
- Vintage fuzz: `gain = 50.0`
- Modern fuzz: `gain = 100.0`
- Extreme fuzz: `gain = 500.0`

### Bitcrusher

| Parameter | Min | Typical | Max | Effect |
|-----------|-----|---------|-----|--------|
| Bit Depth | 1 | 8 | 16 | Extreme → Clean |
| Sample Rate | 2000 Hz | 8000 Hz | 44100 Hz | Extreme → Clean |

**Recommended starting points:**
- Subtle lo-fi: `12-bit, 22 kHz`
- 8-bit game sound: `8-bit, 8 kHz`
- Extreme crush: `4-bit, 4 kHz`

---

## Signal Flow Diagrams

### Overdrive Processing Chain

```
Input x(t)
    ↓
[Pre-Gain Stage]
  x_gained = gain × x(t)
    ↓
[Soft Clipping]
  y = tanh(x_gained)
    ↓
[Tone Shaping / EQ]
  (low-pass filter, typically)
    ↓
[Output Level]
  output = level × y
    ↓
Output y(t)
```

### Distortion Processing Chain

```
Input x(t)
    ↓
[High Pre-Gain Stage]
  x_gained = high_gain × x(t)
    ↓
[Hard Clipping]
  y = clip(x_gained, -T, +T)
    ↓
[Aggressive Tone Shaping]
  (filter control, mid scoop)
    ↓
[Output Level]
  output = level × y
    ↓
Output y(t)
```

### Fuzz Processing Chain

```
Input x(t)
    ↓
[Extreme Pre-Gain]
  x_gained = extreme_gain × x(t)
    ↓
[Square Wave Clipping]
  y = tanh(very_high_gain × x_gained)
    ↓
[Minimal Filtering]
  (preserve harmonics)
    ↓
[Output Level]
  output = level × y
    ↓
Output y(t)
```

### Bitcrusher Processing Chain

```
Input x(t)
    ↓
[Sample Rate Reduction]
  x_downsampled = downsample(x, factor)
    ↓
[Bit Depth Reduction]
  y = quantize(x_downsampled, n_bits)
    ↓
[Optional Dithering]
  y = y + noise
    ↓
Output y(t)
```

---

## Frequency Domain Analysis

### Harmonic Content Generated

**Input: Pure sine wave (440 Hz)**

After processing, each effect generates different harmonics:

#### Overdrive (Soft Clipping)
```
Fundamental: 440 Hz (strongest)
3rd harmonic: 1320 Hz (medium)
5th harmonic: 2200 Hz (weak)
7th harmonic: 3080 Hz (very weak)
Even harmonics: minimal
```

#### Distortion (Hard Clipping)
```
Fundamental: 440 Hz (strong)
2nd harmonic: 880 Hz (medium)
3rd harmonic: 1320 Hz (strong)
4th harmonic: 1760 Hz (medium)
Higher harmonics: present
```

#### Fuzz (Square Wave)
```
Fundamental: 440 Hz (strong)
3rd harmonic: 1320 Hz (very strong)
5th harmonic: 2200 Hz (very strong)
7th harmonic: 3080 Hz (strong)
All odd harmonics present
Even harmonics: minimal
```

#### Bitcrusher
```
Fundamental: 440 Hz
Inharmonic content (aliasing)
Frequency-folding artifacts
Quantization noise
Non-musical overtones
```

---

## Practical Implementation Notes

### 1. Oversampling (Reduces Aliasing)

For digital implementation, oversample before applying nonlinear distortion:

```python
def overdrive_with_oversampling(x, gain=5.0, oversample_factor=4):
    # Upsample
    x_upsampled = scipy.signal.resample(x, len(x) * oversample_factor)

    # Apply distortion
    y_upsampled = np.tanh(gain * x_upsampled)

    # Downsample back
    y = scipy.signal.resample(y_upsampled, len(x))

    return y
```

**Benefits:**
- Reduces aliasing artifacts
- Smoother distortion sound
- More analog-like character

### 2. Pre/Post Filtering

Most real pedals include filtering:

```python
def overdrive_with_filtering(x, gain=5.0, cutoff_freq=5000, sample_rate=44100):
    from scipy.signal import butter, filtfilt

    # Apply overdrive
    y = np.tanh(gain * x)

    # Post-distortion low-pass filter
    nyquist = sample_rate / 2
    normalized_cutoff = cutoff_freq / nyquist
    b, a = butter(2, normalized_cutoff, btype='low')
    y_filtered = filtfilt(b, a, y)

    return y_filtered
```

### 3. DC Offset Removal

Asymmetrical clipping can introduce DC offset:

```python
def remove_dc_offset(x):
    return x - np.mean(x)
```

---

## Conclusion

These mathematical models provide the foundation for understanding and implementing guitar distortion effects. Key points:

1. **Overdrive** = Soft, smooth saturation (tanh, arctan)
2. **Distortion** = Hard, abrupt clipping (clip function, diode model)
3. **Fuzz** = Extreme saturation approaching square wave (very high gain tanh)
4. **Bitcrusher** = Digital quantization (bit reduction, sample rate reduction)

For best results:
- Use oversampling to reduce aliasing
- Add pre/post filtering for more realistic tone
- Experiment with parameter ranges
- Consider asymmetrical clipping for richer harmonics

---

**Document Version:** 1.0
**Last Updated:** 2026-01-05
**Category:** DSP Mathematical Models
**Related Documents:**
- `gain_distortion_types.md` - Conceptual overview of distortion types
- `signal_chain_fundamentals.md` - Signal chain basics

**References:**
- Digital Signal Processing (DSP) literature
- DAFX - Digital Audio Effects (Zölzer)
- The Art of VA Filter Design (Vadim Zavalishin)
- Musical Applications of Microprocessors (Chamberlin)
