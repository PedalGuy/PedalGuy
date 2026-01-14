# 4 个 Amps 信号链完整设计方案

**版本:** 1.0
**建立日期:** 2026-01-15
**配置基础:** 4 个 Amps + 11 个 Pedals（最新全局优化）
**使用场景优先级:** 家里练习 > 家中录音 > 演出 > 立体声

---

## 目录

1. [当前配置概述](#当前配置概述)
2. [方案 A：过渡期方案（保留 4 个 Amps）](#方案-a过渡期方案保留-4-个-amps)
3. [方案 B：最终方案（淘汰 JC-22，保留 3 个）](#方案-b最终方案淘汰-jc-22保留-3-个)
4. [各场景详细信号链](#各场景详细信号链)
5. [Amp 角色分工总结](#amp-角色分工总结)
6. [最终推荐](#最终推荐)

---

## 当前配置概述

### 4 个 Amps 规格对比

| Amp | 类型 | 喇叭 | FX Loop | 输出 | 核心特性 |
|-----|------|------|---------|------|---------|
| **DSM Dumblifier** | Amp-in-a-box | ❌ 无 | ✅ Stereo | XLR + TRS + HP | Dumble ODS, Cab sim, Reverb |
| **Tone King Imperial** | Tube preamp | ❌ 无 | ✅ Stereo | XLR + TRS + HP | 15 IRs, MIDI, 4CM |
| **Roland JC-22** | Solid-state | ✅ 2x6.5" stereo | ✅ Stereo | 1/4" | JC Chorus, Ultra-clean |
| **De Cillia Special 25** | Tube combo | ✅ 1x12" mono | ✅ Mono | Line Out | Class A, Dual ch, KT150 |

### 11 个 Pedals 配置（全局优化后）

**Always-on (3):**
- Empress MKII - Transparent compression
- PA-1QG - 10-band EQ + Boost
- Empress Buffer++ - Signal routing

**Overdrive Stack (5):**
- KOT (From Yesterday) - Foundation transparent OD ⭐
- PRS Horsemeat - Klon-inspired
- Sweet Honey - Neo Soul warm OD
- ODL-1 CS - Dumble-style dual channel
- TWA Source Code - TS evolution

**Time-based (3):**
- FF-1Y - Delay
- Nucleo - Stereo Reverb
- AASB - Shimmer Reverb

### 使用场景优先级

1. **家里练习** ⭐⭐⭐⭐⭐（最重要）
2. **家中录音** ⭐⭐⭐⭐
3. **演出** ⭐⭐⭐
4. **立体声** ⭐⭐（中等重要，可能保留）

---

## 方案 A：过渡期方案（保留 4 个 Amps）

### 核心理念

**4 个 Amps 各司其职，不同场景使用不同组合**

### Amp 角色分工

| Amp | 主要场景 | 次要场景 | 理由 |
|-----|---------|---------|------|
| **Special 25** | 家里练习 ⭐ | 演出 | 真空管 Class A，可调功率（4W/10W/25W），内建 Overdrive |
| **DSM Dumblifier** | 家中录音 ⭐ | 夜间练习 | Silent recording，Dumble ODS，Headphone out |
| **Tone King Imperial** | 家中录音（备选） | 4CM | 15 IRs，MIDI presets，多样性 |
| **Roland JC-22** | 演出（需要 stereo） | - | Stereo speakers，JC Chorus，轻便 |

---

### 场景 1：家里练习（日常，最常用）⭐⭐⭐⭐⭐

#### 方案 1A：Special 25 直接练习（推荐）

**优势：**
- ✅ 真空管 Class A 音色
- ✅ 可调功率（4W 适合家里）
- ✅ 内建 Overdrive（减少 pedals）
- ✅ 真实喇叭反馈

**信号链：**

```
🎸 Guitar
  ↓
① PA-1QG (Always-On EQ + Boost)
  ↓
② Empress MKII (Transparent Compression)
  ↓
③ Buffer++ Input
  ↓
┌─────────────────────────────────────────┐
│ 根据风格选择 Loop                        │
├─────────────────────────────────────────┤
│ 【Loop 1 - Clean/Jazz/Neo Soul】        │
│  KOT → Sweet Honey → Horsemeat          │
│                                         │
│ 【Loop 2 - Rock/Fusion/Blues】          │
│  KOT → Source Code → ODL-1 CS           │
└─────────────────────────────────────────┘
  ↓
Buffer++ Output
  ↓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
【Special 25 - 功率设定 4W】
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Special 25 Input (Clean or Drive channel)
  ↓
Special 25 FX Send (mono)
  ↓
空间系 [FF-1Y → Nucleo (mono mode)] ⚠️ 失去 stereo
  ↓
Special 25 FX Return
  ↓
🔊 Special 25 Speaker (1x12")
```

**设定建议：**
- Special 25 功率：**4W**（适合家里，已经很大声）
- Special 25 通道：
  - Clean 练习：使用 Clean channel + pedals
  - Drive 练习：使用 Drive channel（减少 pedals）

**Pedal 简化（Drive channel 时）：**
- 可以跳过 ODL-1 CS / Source Code
- 直接用 Special 25 内建 Drive

---

#### 方案 1B：夜间静音练习（Headphone）

**优势：**
- ✅ 完全静音（不打扰家人）
- ✅ Stereo 立体声（DSM/Imperial）
- ✅ 专业录音级音质

**方案 1B-1：使用 DSM Dumblifier**

```
Guitar → PA-1QG → Empress MKII → Buffer++
  ├─ Loop 1/2 (Pedals)
  └─ Buffer++ Output
       ↓
DSM Dumblifier Input
  ↓
DSM Preamp (Clean/Overdrive)
  ↓
DSM FX Send (mono)
  ↓
空间系 [FF-1Y → Nucleo (stereo)] ✅ Stereo 保留
  ↓
DSM FX Return (L/R stereo)
  ↓
DSM Headphone Output 🎧
```

**优势：**
- ✅ Dumble ODS 音色
- ✅ Stereo reverb/delay
- ✅ 内建 cab sim（真实音箱感）

---

**方案 1B-2：使用 Tone King Imperial**

```
Guitar → PA-1QG → Empress MKII → Buffer++
  ├─ Loop 1/2 (Pedals)
  └─ Buffer++ Output
       ↓
Tone King Imperial Input
  ↓
Imperial Preamp (Clean/Lead channel)
  ↓
Imperial FX Send (mono)
  ↓
空间系 [FF-1Y → Nucleo (stereo)] ✅ Stereo 保留
  ↓
Imperial FX Return (L/R stereo)
  ↓
Imperial Headphone Output 🎧
```

**优势：**
- ✅ 真空管音色
- ✅ 15 种 IR cab sim
- ✅ MIDI presets（可切换音色）
- ✅ Stereo reverb/delay

---

### 场景 2：家中录音（Silent Recording）⭐⭐⭐⭐

#### 方案 2A：DSM Dumblifier（Dumble 音色专用）

**最佳用途：**
- ✅ Dumble ODS 专业录音
- ✅ Zero latency（全类比）
- ✅ 已验证音质（"best pedal to date"）

**信号链：**

```
Guitar → PA-1QG → Empress MKII → Buffer++
  ├─ Loop 1/2 (根据风格)
  └─ Buffer++ Output
       ↓
DSM Dumblifier Input
  ↓
DSM Preamp (Clean/Overdrive)
  ↓
DSM FX Send (mono)
  ↓
空间系 [AASB → Nucleo → FF-1Y] ✅ Stereo
  ↓
DSM FX Return (L/R stereo)
  ↓
DSM Power Amp + Cab Sim ⭐
  ↓
DSM XLR L/R (Stereo balanced)
  ↓
🎚️ Audio Interface → DAW
```

**录音设定：**
- Cab Sim：选择适合风格的喇叭类型（G12M/G12H/EV12L）
- Reverb：Room/Ethereal/Plate（或使用外部 Nucleo）
- 立体声：✅ 完整保留

---

#### 方案 2B：Tone King Imperial（多样性录音）

**最佳用途：**
- ✅ 15 种专业 IR（多样性）
- ✅ MIDI presets（快速切换音色）
- ✅ 可载入自定义 IR
- ✅ 真空管 preamp

**信号链：**

```
Guitar → PA-1QG → Empress MKII → Buffer++
  ├─ Loop 1/2 (根据风格)
  └─ Buffer++ Output
       ↓
Tone King Imperial Input
  ↓
Imperial Preamp (Clean/Lead + 12AX7 tubes)
  ↓
Imperial FX Send (mono)
  ↓
空间系 [AASB → Nucleo → FF-1Y] ✅ Stereo
  ↓
Imperial FX Return (L/R stereo)
  ↓
Imperial Power Amp Sim + IR Cab Sim ⭐
  ↓
Imperial XLR L/R (Stereo balanced)
  ↓
🎚️ Audio Interface → DAW
```

**录音设定：**
- IR Selection：15 种 OwnHammer IRs 可选
- MIDI：可储存不同风格的 presets
- 立体声：✅ 完整保留

---

#### 录音选择建议

| 需求 | 推荐 Amp | 理由 |
|------|---------|------|
| **Dumble 音色** | DSM Dumblifier | 专精 Dumble ODS，评测最高 |
| **多样性** | Tone King Imperial | 15 种 IRs，MIDI presets |
| **快速切换** | Tone King Imperial | MIDI 可程式化 |
| **真空管染色** | Tone King Imperial | 12AX7 tubes |
| **零延迟** | DSM Dumblifier | 全类比，zero latency |

**可以两个都用：**
- Track 1-3: DSM (Dumble 音色)
- Track 4-6: Imperial (其他音色)

---

### 场景 3：演出 ⭐⭐⭐

#### 方案 3A：Special 25（真空管舞台音色）

**最佳用途：**
- ✅ 真空管 Class A 音色
- ✅ 功率充足（25W ≈ 50W solid-state）
- ✅ 内建 Overdrive
- ✅ 10 年保固

**信号链：**

```
Guitar → PA-1QG → Empress MKII → Buffer++
  ├─ Loop 2 (Rock/Fusion/Blues)
  │  KOT → Source Code → ODL-1 CS (可选)
  └─ Buffer++ Output
       ↓
Special 25 Input (Clean or Drive)
  ↓
Special 25 FX Send (mono)
  ↓
空间系 [FF-1Y → Nucleo (mono)] ⚠️ Mono only
  ↓
Special 25 FX Return
  ↓
🔊 Special 25 Speaker (1x12")
```

**舞台设定：**
- 功率：25W（full power）
- 通道：根据歌曲选择 Clean/Drive
- Pedals：简化配置，减少踏板切换

**劣势：**
- ⚠️ Mono only（失去 stereo）
- ⚠️ 重量重（18kg）
- ⚠️ 无 DI out（如需 PA 需要麦克风）

---

#### 方案 3B：JC-22（Stereo 立体声舞台）⚠️

**最佳用途：**
- ✅ Stereo speakers（立体声音场）
- ✅ JC Chorus（传奇音色）
- ✅ 轻便（12kg）

**信号链：**

```
Guitar → PA-1QG → Empress MKII → Buffer++
  ├─ Loop 1 (Clean/Jazz/Neo Soul)
  │  KOT → Sweet Honey → Horsemeat
  └─ Buffer++ Output
       ↓
JC-22 Input
  ↓
JC-22 FX Send (stereo)
  ↓
空间系 [FF-1Y → Nucleo (stereo)] ✅ Stereo 完整
  ↓
JC-22 FX Return L/R
  ↓
🔊 JC-22 Speakers (2x6.5" stereo)
```

**舞台设定：**
- JC Chorus：ON（传奇音色）
- Pedals：完整 OD stack（JC-22 是 clean platform）

**劣势：**
- ⚠️ 功率小（30W，中小型场地）
- ⚠️ 需要完整 pedal chain（无内建 overdrive）

---

#### 演出选择建议

| 场地大小 | 音色需求 | 推荐 Amp |
|---------|---------|---------|
| **小型** (Cafe, Bar) | 真空管音色 | Special 25 (4W/10W) |
| **中型** (Live House) | 真空管音色 | Special 25 (25W) |
| **中型** (Live House) | Stereo 立体声 | JC-22 (30W) ⚠️ 可能不够 |
| **大型** | 任何 | DI to PA（DSM/Imperial） |

**Special 25 vs JC-22：**
- 如果看重**真空管音色** → Special 25
- 如果看重**Stereo 立体声** → JC-22
- 如果两者都要 → 可能需要两台 amp（过渡期保留）

---

### 场景 4：立体声（Stereo）⭐⭐

#### 支持 Stereo 的 Amps

| Amp | Stereo 能力 | 说明 |
|-----|------------|------|
| **DSM Dumblifier** | ✅ Full stereo | FX loop stereo, Output stereo |
| **Tone King Imperial** | ✅ Full stereo | FX loop stereo, XLR stereo |
| **Roland JC-22** | ✅ Full stereo | FX loop stereo, Speakers stereo |
| **Special 25** | ❌ Mono only | FX loop mono, Speaker mono |

#### Stereo 使用建议

**如果 Stereo 很重要：**
- **录音：** 使用 DSM 或 Imperial（XLR stereo）
- **练习：** 使用 DSM 或 Imperial（Headphone stereo）
- **演出：** 使用 JC-22（Speakers stereo）或 DI to PA

**如果可以接受 Mono：**
- **练习/演出：** 使用 Special 25
- **Nucleo/FF-1Y：** 设定为 mono mode

---

## 方案 B：最终方案（淘汰 JC-22，保留 3 个）

### 核心理念

**如果最终决定淘汰 JC-22，保留 Special 25 作为唯一舞台 amp**

### 淘汰 JC-22 的理由

1. **Special 25 更强大**
   - ✅ 真空管 Class A 音色（JC-22 是 solid-state）
   - ✅ 内建 Overdrive（JC-22 需要 pedals）
   - ✅ 功率更大（25W tube ≈ 50W ss vs 30W）

2. **Stereo 可以靠其他 amp**
   - DSM/Imperial 提供 stereo 录音
   - 演出可以 DI to PA（stereo）

3. **减少设备**
   - 4 个 → 3 个 Amps
   - 简化选择，减少决策负担

### 妥协

- ⚠️ 失去 JC Chorus 传奇音色
- ⚠️ 失去 stereo speakers 舞台体验
- ⚠️ 演出时 Nucleo/FF-1Y 只能用 mono

---

### 最终 3 个 Amps 角色分工

| Amp | 主要场景 | 次要场景 | 理由 |
|-----|---------|---------|------|
| **Special 25** | 家里练习 ⭐ | 演出 ⭐ | 真空管 Class A，万能 |
| **DSM Dumblifier** | 家中录音 ⭐ | 夜间练习 | Dumble ODS，Silent recording |
| **Tone King Imperial** | 家中录音（多样性） | 4CM | 15 IRs，MIDI，真空管 preamp |

---

### 各场景信号链（最终方案）

#### 场景 1：家里练习

**使用：Special 25**（同方案 A）

```
Guitar → PA-1QG → Empress MKII → Buffer++ → [Pedals] → Special 25
  ↓
Special 25 FX Loop [FF-1Y → Nucleo (mono)]
  ↓
🔊 Speaker (1x12")
```

- 功率：4W/10W（根据时间调整）
- 通道：Clean + pedals 或 Drive（简化）

---

#### 场景 2：家中录音

**使用：DSM（Dumble）或 Imperial（多样性）**（同方案 A）

```
【DSM 录音】
Guitar → [Pedals] → DSM → FX Loop [空间系 stereo] → XLR L/R → Interface

【Imperial 录音】
Guitar → [Pedals] → Imperial → FX Loop [空间系 stereo] → XLR L/R → Interface
```

- ✅ Stereo 完整保留

---

#### 场景 3：演出

**使用：Special 25**（真空管舞台音色）

```
Guitar → PA-1QG → Empress MKII → Buffer++ → [Pedals] → Special 25
  ↓
Special 25 FX Loop [FF-1Y → Nucleo (mono)] ⚠️
  ↓
🔊 Speaker (1x12")
```

- 功率：25W full power
- 妥协：Mono only，失去 stereo 立体声

**如需 DI to PA：**
```
Special 25 Line Out (160Ω) → DI Box → PA System
```
或
```
Special 25 Speaker → Microphone → PA System
```

---

#### 场景 4：夜间静音练习

**使用：DSM 或 Imperial（Headphone）**

```
Guitar → [Pedals] → DSM/Imperial → FX Loop [空间系 stereo] → Headphone 🎧
```

- ✅ Stereo 完整保留

---

## 各场景详细信号链

### 完整 Pedal Chain 结构

所有场景都使用这个基础 pedal chain：

```
🎸 Guitar
  ↓
① PA-1QG (Always-On EQ + Boost)
  ↓
② Empress MKII (Always-On Compression)
  ↓
③ Empress Buffer++ Input
  ↓
┌─────────────────────────────────────────────────┐
│ Buffer++ Loop Select (根据音乐风格选择)          │
├─────────────────────────────────────────────────┤
│                                                 │
│ 【Loop 1 - Clean/Jazz/Neo Soul】                │
│  ├─ KOT (Yellow Clean boost, Always-on)        │
│  ├─ Sweet Honey (温暖 OD, 可选)                │
│  ├─ Horsemeat (Klon boost, 可选)               │
│  └─ CE-2W (Chorus, 可选)                        │
│                                                 │
│                 或                              │
│                                                 │
│ 【Loop 2 - Rock/Fusion/Blues】                  │
│  ├─ KOT (Dual OD, Yellow + Red)                │
│  ├─ Source Code (TS 中频, 可选)                │
│  └─ ODL-1 CS (Dumble, 可选)                    │
│                                                 │
└─────────────────────────────────────────────────┘
  ↓
Buffer++ Output
  ↓
[进入对应的 Amp]
```

---

### 空间系效果配置

```
【Amp FX Send】
  ↓
④ AASB (Shimmer Reverb, 可选)
  ↓
⑤ Nucleo (Main Reverb, stereo/mono 可切换)
  ↓
⑥ FF-1Y (Delay, stereo/mono 可切换)
  ↓
【Amp FX Return】
```

**Stereo/Mono 设定：**
- Special 25：Mono mode（FX loop 只有 mono）
- DSM/Imperial/JC-22：Stereo mode（完整立体声）

---

## Amp 角色分工总结

### 方案 A：过渡期（4 个 Amps 全保留）

| Amp | 练习 | 录音 | 演出 | 夜间练习 | 优势 |
|-----|------|------|------|---------|------|
| **Special 25** | ⭐⭐⭐⭐⭐ | ❌ | ⭐⭐⭐⭐⭐ | ❌ | 真空管，可调功率，内建 OD |
| **DSM** | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐ (DI) | ⭐⭐⭐⭐⭐ | Dumble ODS，Silent，Stereo |
| **Imperial** | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐ (DI) | ⭐⭐⭐⭐⭐ | 15 IRs，MIDI，真空管 |
| **JC-22** | ⭐⭐ | ❌ | ⭐⭐⭐⭐ | ❌ | Stereo speakers，JC Chorus |

**使用建议：**
- **日常练习（白天）：** Special 25（4W/10W）
- **夜间练习：** DSM 或 Imperial（Headphone）
- **录音（Dumble）：** DSM
- **录音（多样性）：** Imperial
- **演出（真空管）：** Special 25
- **演出（Stereo）：** JC-22

---

### 方案 B：最终方案（淘汰 JC-22，保留 3 个）

| Amp | 练习 | 录音 | 演出 | 夜间练习 | 优势 |
|-----|------|------|------|---------|------|
| **Special 25** | ⭐⭐⭐⭐⭐ | ❌ | ⭐⭐⭐⭐⭐ | ❌ | 万能舞台 amp |
| **DSM** | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐ (DI) | ⭐⭐⭐⭐⭐ | Dumble 专用录音 |
| **Imperial** | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐ (DI) | ⭐⭐⭐⭐⭐ | 多样性录音 |

**使用建议：**
- **日常练习（白天）：** Special 25（4W/10W）
- **夜间练习：** DSM 或 Imperial（Headphone）
- **录音：** DSM（Dumble）或 Imperial（多样性）
- **演出：** Special 25（mono，失去 stereo）

**妥协：**
- ⚠️ 失去 JC-22 stereo speakers
- ⚠️ 失去 JC Chorus 传奇音色
- ⚠️ 演出时 mono only

---

## 最终推荐

### 🏆 推荐：方案 A（过渡期，保留 4 个 Amps）

#### 推荐理由

1. **满足所有场景需求**
   - ✅ 练习：Special 25（真空管，可调功率）
   - ✅ 录音：DSM + Imperial（Stereo，多样性）
   - ✅ 演出：Special 25（真空管）或 JC-22（Stereo）
   - ✅ 夜间：DSM/Imperial（Headphone，Stereo）

2. **Stereo 选项保留**
   - 录音：DSM/Imperial 完整 stereo
   - 演出：JC-22 stereo speakers（如需要）
   - 练习：DSM/Imperial headphone stereo

3. **灵活性最大**
   - 真空管音色：Special 25 + Imperial
   - Dumble 音色：DSM + ODL-1 CS
   - Stereo 音色：DSM/Imperial/JC-22
   - 各 amp 各司其职，零浪费

4. **匹配您的优先级**
   - 练习 ⭐⭐⭐⭐⭐ → Special 25 完美
   - 录音 ⭐⭐⭐⭐ → DSM/Imperial 双重选择
   - 演出 ⭐⭐⭐ → Special 25 或 JC-22
   - 立体声 ⭐⭐ → 可选择保留（录音/夜间练习用）

---

### ⏰ 过渡到方案 B 的时机

**何时考虑淘汰 JC-22？**

满足以下条件时：

1. ✅ **Stereo 演出需求减少**
   - 如果您很少需要 stereo speakers 舞台表演
   - 或可以接受 Special 25 的 mono 演出

2. ✅ **真空管音色成为主要需求**
   - Special 25 的 Class A 音色成为您的首选
   - JC-22 的 solid-state 音色使用频率降低

3. ✅ **希望简化设备**
   - 4 个 amp 管理太复杂
   - 想要更专注的配置

4. ✅ **JC Chorus 需求降低**
   - 如果您很少使用 JC Chorus
   - 或可以用 CE-2W 替代

---

### 📋 使用决策流程图

```
开始
  ↓
现在是什么场景？
  ↓
┌───────────────────────────────────────────────┐
│ 1. 家里练习（日常）                            │
│    ├─ 白天 → Special 25 (4W/10W)              │
│    └─ 夜间 → DSM/Imperial (Headphone)         │
│                                               │
│ 2. 家中录音                                   │
│    ├─ Dumble 音色 → DSM (XLR stereo)         │
│    └─ 多样性/MIDI → Imperial (XLR stereo)    │
│                                               │
│ 3. 演出                                       │
│    ├─ 需要真空管 → Special 25 (25W, mono)    │
│    ├─ 需要 Stereo → JC-22 (30W, stereo) ⚠️  │
│    └─ 大型场地 → DI to PA (DSM/Imperial)     │
│                                               │
│ 4. 夜间静音练习                                │
│    └─ DSM/Imperial (Headphone, stereo)       │
└───────────────────────────────────────────────┘
```

---

## 附录：快速设定参考

### Special 25 功率设定

| 场景 | 功率 | 说明 |
|------|------|------|
| **家里练习（白天）** | 4W | 已经很大声，适合公寓 |
| **家里练习（周末）** | 10W | 可以更放开 |
| **演出（小型）** | 10W | Cafe, Bar |
| **演出（中型）** | 25W | Live House |

### Nucleo/FF-1Y 设定

| 使用 Amp | Stereo/Mono | 说明 |
|---------|------------|------|
| **Special 25** | Mono | FX loop 只有 mono |
| **DSM** | Stereo | 完整 stereo FX loop |
| **Imperial** | Stereo | 完整 stereo FX loop |
| **JC-22** | Stereo | 完整 stereo FX loop |

### Pedal Chain 简化建议

**Special 25 Drive Channel 使用时：**
- 可以跳过 ODL-1 CS（内建 drive 已足够）
- 可以跳过 Source Code（如果不需要 TS 中频）
- 保留 KOT（Foundation OD）

**录音时（DSM/Imperial）：**
- 使用完整 pedal chain
- 根据风格选择 Loop 1 或 Loop 2

---

**报告版本:** 1.0
**建立日期:** 2026-01-15
**下次更新:** 根据实际使用体验调整

**相关文件:**
- `pedal_configuration_optimization_2026-01-14.md` - 11 个 Pedals 全局优化
- `amp_configuration_analysis_2026-01-14.md` - 4 个 Amps 完整分析
- `dumblifier_integration_evaluation.md` - Dumblifier 整合评估（v2.0）
