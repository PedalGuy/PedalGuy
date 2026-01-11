# Emil 吉他訊號鏈配置 - Toneking Only 版本

**版本:** Toneking Only v1.0
**建立日期:** 2026-01-08
**基於:** V3.0 (2025-12-30) 改進版
**核心變更:** 移除 JC-22，只使用 Tone King Imperial MKII Preamp Pedal

---

## 設計理念

### 核心目標

**從雙音箱配置 (JC-22 + Toneking) 轉換為單 Preamp Pedal 配置**

- ✅ 保留原本訊號鏈的豐富度（90%+ 音色品質）
- ✅ 使用 Empress Buffer++ 實現雙訊號鏈切換
- ✅ 補償 JC-22 的 Dimensional Space Chorus
- ✅ 充分發揮 Toneking 的 Stereo FX Loop + XLR 錄音輸出
- ✅ 實現 MIDI 完整控制（PA-1QG + ODL-1-CS）

### 關鍵策略

1. **Chorus 補償**
   - 新增 **Boss CE-2W Waza Craft Chorus**
   - CE-1 模式 = JC-120 Chorus 來源
   - 完全替代 JC-22 的 Dimensional Space Chorus

2. **雙訊號鏈實現**
   - 使用 **Empress Buffer++ Mode 5 (Loop Select)**
   - Loop 1: Clean/Jazz/Neo Soul 訊號鏈
   - Loop 2: Rock/Fusion/Post Rock 訊號鏈
   - 腳踏切換，即時響應

3. **Toneking 雙通道應用**
   - **Rhythm Channel (Clean)** → Loop 1 使用
   - **Lead Channel (Overdrive)** → Loop 2 使用
   - 用音箱通道區分音樂風格

4. **Stereo XLR 錄音**
   - Toneking Stereo FX Return (L/R)
   - Toneking Stereo XLR Outputs (L/R)
   - 直接輸出到 Audio Interface
   - 專業級 stereo 錄音能力

5. **優化的空間系順序**
   - AASB (Mono) → Nucleo (創造 Stereo) → FF-1Y (保留 Stereo)
   - 訊號流程從 Mono 逐漸展開為完整 Stereo
   - 最大化立體聲空間感
   - Reverb → Delay 順序適合 Post Rock/Ambient

---

## 核心設備清單

### 新增設備（相較於 V3.0）

| 設備 | 用途 | 價格 | 必要性 |
|------|------|------|--------|
| ⭐ **Boss CE-2W Waza Craft Chorus** | 替代 JC-22 Chorus | $180-200 | 🔥 **必需** |
| ✅ **Empress Buffer++** | 雙訊號鏈路由切換 | $299 | ✅ **強烈建議** |
| ✅ **Rockboard MOD 2 V2** | Patchbay + MIDI 管理 | $150-180 | ✅ **強烈建議** |

### 完整效果器清單（14顆）

#### 【Always-On】1顆
1. ✅ **Free the Tone PA-1QG** ($425)
   - EQ + Clean Boost
   - 99 Preset，MIDI 支援
   - 為每把吉他建立專用 EQ

---

#### 【Utility】1顆
2. ✅ **Empress Buffer++** ($299)
   - 12 種路由模式
   - Loop 1 & Loop 2 切換
   - Stereo 能力

---

#### 【Loop 1 - Clean/Jazz/Neo Soul】4顆

3. ✅ **Empress MKII Compressor** ($219)
   - 極度透明壓縮
   - 保持撥弦動態

4. ✅ **Mad Professor Sweet Honey Deluxe** ($220)
   - 溫暖 Neo Soul 核心 OD

5. ✅ **PRS Horsemeat**
   - Klon-style 透明 Boost

6. ⭐ **Boss CE-2W Waza Craft Chorus** ($180-200) **【新增】**
   - 替代 JC-22 Dimensional Space Chorus
   - CE-1 模式 = JC-120 Chorus
   - Stereo 輸出

---

#### 【Loop 2 - Rock/Fusion/Post Rock】5顆

7. ✅ **Origin Effects Cali76 FET** ($369)
   - 染色壓縮 + Sustain
   - Post Rock 延音

8. ✅ **Roshi Blacklon** ($200)
   - Amp-in-a-Box (Blackface 模擬)

9. ✅ **JHS Morning Glory V3**
   - Bluesbreaker Overdrive

10. ✅ **TWA Source Code** ($299)
    - TS Evolution 中頻突出

11. ✅ **Free the Tone ODL-1-CS** ($425)
    - Dumble 雙通道高階音色

---

#### 【空間系 Pedalboard - 獨立放置】3顆

12. ✅ **Lichtlaerm AASB** ($225)
    - Shimmer/Drone 雙向八度
    - Mono In/Out

13. ✅ **Cornerstone Nucleo** ($350)
    - Stereo 主 Reverb
    - Reactor 核電廠模式
    - Mono In/Stereo Out

14. ✅ **Free the Tone FF-1Y** ($400)
    - Realtime BPM Analyzer Delay
    - Stereo In/Out

---

## 完整訊號鏈架構圖

```
🎸 吉他
  ↓
【MOD 2 V2 TRS 1 - Input】
  ↓
① PA-1QG (Always-On EQ + Clean Boost)
   ┌─────────────────────────────────────┐
   │ • 99 Preset MIDI 控制                │
   │ • Preset 1-4: 不同吉他專用 EQ        │
   │ • Preset 5-7: Solo Boost             │
   │ • LEVEL 功能: Clean Boost            │
   └─────────────────────────────────────┘
  ↓
② Empress Buffer++ Input
  ↓
┌─────────────────────────────────────────────────┐
│ Buffer++ 內部路由 (Mode 5: Loop Select)         │
│ 用腳踏切換 Loop 1 或 Loop 2                     │
├─────────────────────────────────────────────────┤
│                                                  │
│ 【Loop 1 - Clean/Jazz/Neo Soul 訊號鏈】          │
│  ├─ ③ Empress MKII (透明壓縮)                   │
│  ├─ ④ Sweet Honey (溫暖 OD)                     │
│  ├─ ⑤ PRS Horsemeat (Klon Boost)                │
│  └─ ⑥ Boss CE-2W (Chorus) ⭐ 新增                │
│                                                  │
│              或 (腳踏切換)                        │
│                                                  │
│ 【Loop 2 - Rock/Fusion/Post Rock 訊號鏈】        │
│  ├─ ③ Cali76 FET (染色壓縮 + Sustain)           │
│  ├─ ④ Roshi Blacklon (Amp-in-a-Box)             │
│  ├─ ⑤ JHS Morning Glory (BB OD)                 │
│  ├─ ⑥ TWA Source Code (TS Evolution)            │
│  └─ ⑦ ODL-1-CS (Dumble)                         │
│                                                  │
└─────────────────────────────────────────────────┘
  ↓
Buffer++ Output
  ↓
【MOD 2 V2 TRS 2 - Output】
  ↓
🎛️ Tone King Imperial MKII Input
  ↓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
【Toneking Preamp 處理】
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  ↓
  Loop 1 使用：Rhythm Channel (Clean)
  Loop 2 使用：Lead Channel (Overdrive)
  ↓
Toneking FX Send (mono)
  ↓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
【空間系 Pedalboard - 獨立放置】
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  ↓
⑧ Lichtlaerm AASB (Shimmer) - Mono In/Out
  ↓
⑨ Cornerstone Nucleo (Reverb) - Mono In/Stereo Out
  ↓
⑩ Free the Tone FF-1Y (Delay) - Stereo In/Out
  ↓
Toneking FX Return (L/R stereo)
  ↓
Toneking Preamp 最終混合
  ↓
Toneking XLR Output L/R (stereo)
  ↓
🎚️ Audio Interface XLR Input L/R
```

---

## 訊號鏈 1：Clean / Jazz / Neo Soul / Funk

**目標音樂類型**：Jazz, Neo Soul, Funk, Pop Rock
**主要吉他**：Greco TE-500, Fender Tokyo Thinline, ESP Throbber-CTM
**主要音色**：Clean Tone + 溫暖 OD + Chorus 寬度感
**評分**：★★★★☆ (90/100)

### 完整訊號流程

```
🎸 吉他 (選擇對應 Preset)
  ↓
【MOD 2 V2 - Input】
  ↓
① PA-1QG
   ┌─────────────────────────────────────┐
   │ Preset 配置：                        │
   │                                      │
   │ • Preset 1: ESP EC-CTM               │
   │   - LEVEL: 0dB（高輸出）             │
   │   - EQ: 提升 800Hz-3.2kHz           │
   │                                      │
   │ • Preset 2: Greco TE-500             │
   │   - LEVEL: +3dB（中等輸出）          │
   │   - EQ: 提升 800Hz-3.2kHz           │
   │                                      │
   │ • Preset 3: ESP Throbber-CTM         │
   │   - LEVEL: +6dB（低輸出）            │
   │   - EQ: 平衡中頻                    │
   │                                      │
   │ • Preset 4: Fender Tokyo Thinline    │
   │   - LEVEL: +4dB（中等輸出）          │
   │   - EQ: 提升中高頻                  │
   ├─────────────────────────────────────┤
   │ 目的：為每把吉他建立專用 EQ + Boost  │
   └─────────────────────────────────────┘
  ↓
② Buffer++ Input
  ↓
【Buffer++ Loop 1 Send】
  ↓
③ Empress MKII Compressor
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • INPUT: 低 (1-2 LED)                │
   │ • RATIO: 2:1                         │
   │ • ATTACK: 快                         │
   │ • RELEASE: 中                        │
   │ • TILT EQ: 12點鐘（正午）            │
   │ • MIX: 80-100%                       │
   │ • OUTPUT: 正常                       │
   ├─────────────────────────────────────┤
   │ 目的：極度透明動態控制               │
   │ 效果：保持撥弦動態，輕微控制峰值     │
   └─────────────────────────────────────┘
  ↓
④ Mad Professor Sweet Honey Overdrive Deluxe
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • DRIVE: 11-12點鐘                   │
   │ • FOCUS: 1-2點鐘（Neo Soul 甜蜜點）  │
   │ • VOLUME: 12-1點鐘                   │
   │ • TONE: 12點鐘                       │
   ├─────────────────────────────────────┤
   │ 目的：溫暖 Neo Soul 核心音色         │
   │ 效果：低至中等增益，溫暖甜美         │
   └─────────────────────────────────────┘
  ↓
⑤ PRS Horsemeat
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • DRIVE: 9-10點鐘（低 Gain）         │
   │ • VOLUME: 2點鐘（Boost 模式）        │
   │ • TONE: 12-1點鐘                     │
   ├─────────────────────────────────────┤
   │ 目的：Klon-style 透明 Boost          │
   │ 效果：推動前面 Sweet Honey OD        │
   │ 特性：極度透明，增加中頻穿透力       │
   └─────────────────────────────────────┘
  ↓
⑥ Boss CE-2W Waza Craft Chorus ⭐ 新增
   ┌─────────────────────────────────────┐
   │ ⭐ 關鍵新增：替代 JC-22 Chorus        │
   ├─────────────────────────────────────┤
   │ 設定：                               │
   │ • MODE: CE-1 (Stereo Chorus)         │
   │ • RATE: 慢（類似 JC-22 SPEED 3-4）   │
   │ • DEPTH: 中（類似 JC-22 DEPTH 4-5）  │
   │ • OUTPUT: Stereo L+R                 │
   ├─────────────────────────────────────┤
   │ 目的：替代 JC-22 Dimensional Chorus  │
   │ 效果：Neo Soul 標準寬度感            │
   │ 特性：CE-1 模式 = JC-120 Chorus 來源 │
   │ 使用：Always On（Clean Tone 核心）   │
   └─────────────────────────────────────┘
  ↓
【Buffer++ Loop 1 Return】
  ↓
Buffer++ Output
  ↓
【MOD 2 V2 - Output】
  ↓
🎛️ Tone King Imperial MKII Input
  ↓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
【Toneking Rhythm Channel - Clean】
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
   ┌─────────────────────────────────────┐
   │ 音箱設定：                           │
   │ • CHANNEL: Rhythm (Clean Channel)    │
   │ • VOLUME: 12-1點鐘                   │
   │ • TREBLE: 12點鐘                     │
   │ • MID: 12點鐘                        │
   │ • BASS: 12-1點鐘                     │
   │ • MID-BITE: OFF（保持清晰）          │
   ├─────────────────────────────────────┤
   │ 目的：管機溫暖 + 相對透明            │
   │ 效果：比 JC-22 稍溫暖，但保持清晰    │
   │ 音色：3 x 12AX7 tubes 處理           │
   └─────────────────────────────────────┘
  ↓
Toneking FX Send (mono)
  ↓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
【空間系 Pedalboard】
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  ↓
⑦ Lichtlaerm AASB Shimmer Reverb (Mono In/Out)
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • MODE: Off（Clean/Jazz 不常用）     │
   │ • 需要時可開啟 Above 或 Both         │
   │ • MIX: 30-50%                        │
   ├─────────────────────────────────────┤
   │ 目的：偶爾使用的 Shimmer 效果        │
   │ 效果：增添空靈感（選擇性使用）       │
   │ 輸出：Mono                           │
   └─────────────────────────────────────┘
  ↓
⑧ Cornerstone Nucleo Reverb (Mono In/Stereo Out)
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • MODE: Room/Hall（視場景）          │
   │ • DECAY: 30-50%                      │
   │ • BLEND: 30-50%                      │
   │ • VOICING: Normal                    │
   │ • OUTPUT: Stereo L+R                 │
   │ • RIGHT OUTPUT: Transformer-Isolated │
   │   （避免 Ground Loop）               │
   ├─────────────────────────────────────┤
   │ 目的：創造 Stereo 空間感             │
   │ 效果：豐富空間感，Stereo 寬度        │
   └─────────────────────────────────────┘
  ↓
⑨ Free the Tone FF-1Y Delay (Stereo In/Out)
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • MODE: Digital                      │
   │ • TIME: 視曲目（建議 1/4 note）      │
   │ • FEEDBACK: 3-4 repeats              │
   │ • MIX: 20-40%                        │
   │ • REALTIME BPM ANALYZER: ON          │
   ├─────────────────────────────────────┤
   │ 目的：精準 BPM 同步 Delay            │
   │ 效果：自動偵測節奏，精準同步         │
   │ 輸出：保留並增強 Stereo 寬度         │
   └─────────────────────────────────────┘
  ↓
Toneking FX Return (Stereo L+R)
  ↓
Toneking Preamp 最終混合
  ↓
Toneking XLR Output L/R (stereo)
  ↓
🎚️ Audio Interface XLR Input L/R
```

### 效果器使用統計

| 效果器 | 使用率 | 角色 |
|--------|--------|------|
| PA-1QG | 100% | EQ + Clean Boost |
| Empress MKII | 95% | 透明壓縮 |
| Sweet Honey | 90% | 核心 OD 音色 |
| PRS Horsemeat | 80% | 透明 Klon Boost |
| **CE-2W Chorus** | **100%** | **Chorus 寬度感（新增）** |
| AASB | 20% | Shimmer（選擇性使用） |
| Nucleo | 95% | 主 Reverb + 創造 Stereo |
| FF-1Y | 100% | 主 Delay + 增強 Stereo |

**總計**：8顆效果器（前級5顆 + 空間系3顆）

---

## 訊號鏈 2：Rock / Fusion / Post Rock / Ambient

**目標音樂類型**：Post Rock, Fusion, Ambient, Alternative Rock, Classic Rock
**主要吉他**：ESP EC-CTM, Greco TE-500
**主要音色**：高增益 + Sustain + 複雜音景
**評分**：★★★★★ (96/100)

### 完整訊號流程

```
🎸 吉他 (ESP EC-CTM 或 Greco TE-500)
  ↓
【MOD 2 V2 - Input】
  ↓
① PA-1QG
   ┌─────────────────────────────────────┐
   │ Preset 配置：                        │
   │                                      │
   │ • Preset 5: ESP EC-CTM (Post Rock)   │
   │   - LEVEL: 0dB（高輸出）             │
   │   - EQ: 提升 100Hz-400Hz（厚度）    │
   │                                      │
   │ • Preset 6: Greco TE-500 (Post Rock) │
   │   - LEVEL: +3dB（中等輸出）          │
   │   - EQ: 提升低頻與中高頻            │
   │                                      │
   │ • Preset 7: Solo Boost（通用）       │
   │   - LEVEL: +9dB（大音量 Solo）       │
   │   - EQ: 平坦或提升 800Hz-3.2kHz     │
   ├─────────────────────────────────────┤
   │ 目的：EQ 調整 + 視需求 Boost         │
   └─────────────────────────────────────┘
  ↓
② Buffer++ Input
  ↓
【Buffer++ Loop 2 Send】
  ↓
③ Origin Effects Cali76 FET
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • IN: 中（5-6 LED）                  │
   │ • ATTACK: 快                         │
   │ • RELEASE: 中                        │
   │ • RATIO: 固定 1176 風格              │
   │ • DRY: 70-80%（混入原始訊號）        │
   ├─────────────────────────────────────┤
   │ 目的：                               │
   │ 1. 增加 Sustain（Post Rock 延音）    │
   │ 2. 染色增添管機感                    │
   │ 3. DRY 混合保留撥弦動態              │
   │ 效果：溫暖圓潤，延音豐富             │
   └─────────────────────────────────────┘
  ↓
④ Roshi Blacklon (Amp-in-a-Box)
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • TUBE: 6L6 Mode（Post Rock）        │
   │         6V6 Mode（Fusion）           │
   │ • TONE: Drive Mode（增益模式）       │
   │         Mellow Mode（溫暖模式）      │
   │ • DRIVE: 11-1點鐘                    │
   │ • VOLUME: 12-1點鐘                   │
   ├─────────────────────────────────────┤
   │ 目的：Blackface 管機模擬             │
   │ 效果：為訊號鏈增加管機特性           │
   │ 用途：                               │
   │ • 6L6 + Drive = Post Rock Crunch     │
   │ • 6V6 + Mellow = Fusion 溫暖         │
   └─────────────────────────────────────┘
  ↓
⑤ JHS Morning Glory V3
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • GAIN: 10-12點鐘                    │
   │ • VOLUME: 12-1點鐘                   │
   │ • TONE: 12點鐘                       │
   │ • SWITCH: 根據需求選擇模式           │
   ├─────────────────────────────────────┤
   │ 目的：Bluesbreaker Overdrive         │
   │ 效果：經典 BB 音色，開放清晰         │
   │ 特性：無 clipping 問題，動態自然     │
   └─────────────────────────────────────┘
  ↓
⑥ TWA Source Code (TS Evolution)
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • DRIVE: 10-12點鐘                   │
   │ • TONE: 12-1點鐘                     │
   │ • VOLUME: 12點鐘                     │
   │ • BITE CONTROL: 調整諧波平衡         │
   │   - 逆時針：偶次諧波（溫暖）         │
   │   - 順時針：奇次諧波（明亮）         │
   ├─────────────────────────────────────┤
   │ 目的：                               │
   │ 1. TS-style 中頻突出（800Hz-1.5kHz） │
   │ 2. Bite Control 微調諧波            │
   │ 3. 18V 升壓提供大 headroom           │
   │ 使用時機：                           │
   │ • Classic Rock 需要 TS 中頻時開啟    │
   │ • 其他風格可 Bypass                  │
   │ 效果：TS 特有中頻穿透力              │
   └─────────────────────────────────────┘
  ↓
⑦ Free the Tone ODL-1-CS (Dumble)
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • CHANNEL: Drive Channel             │
   │ • VOLTAGE: 14-16V                    │
   │ • MODE: ROCK Mode                    │
   │ • DRIVE: 10-1點鐘                    │
   │ • VOLUME: 12點鐘                     │
   │ • TONE: 12點鐘                       │
   ├─────────────────────────────────────┤
   │ 目的：Dumble 高階音色                │
   │ 效果：Fusion 經典音色                │
   │ （Larry Carlton, Robben Ford 風格）  │
   └─────────────────────────────────────┘
  ↓
【Buffer++ Loop 2 Return】
  ↓
Buffer++ Output
  ↓
【MOD 2 V2 - Output】
  ↓
🎛️ Tone King Imperial MKII Input
  ↓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
【Toneking Lead Channel - Overdrive】
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
   ┌─────────────────────────────────────┐
   │ 音箱設定：                           │
   │ • CHANNEL: Lead                      │
   │ • GAIN: 10-12點鐘（疊加前級 OD）     │
   │ • VOLUME: 12點鐘                     │
   │ • TREBLE: 12-1點鐘                   │
   │ • MID: 12點鐘                        │
   │ • BASS: 11點鐘                       │
   │ • MID-BITE: ON（增加穿透力）         │
   ├─────────────────────────────────────┤
   │ 目的：管機溫暖 + 增益疊加            │
   │ 效果：Post Rock/Fusion 高增益音色    │
   │ 音色：3 x 12AX7 tubes overdrive      │
   └─────────────────────────────────────┘
  ↓
Toneking FX Send (mono)
  ↓
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
【空間系 Pedalboard】
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  ↓
⑧ Lichtlaerm AASB Shimmer Reverb (Mono In/Out)
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • MODE: Above（高八度）              │
   │         Both（雙向八度）             │
   │ • MIX: 60-90%（大比例 Wet）          │
   │ • DECAY: 長                          │
   │ • FREEZE: 開啟（凍結音景）           │
   ├─────────────────────────────────────┤
   │ 目的：雙向八度 Shimmer/Drone         │
   │ 效果：天堂與地底碰撞的音景           │
   │ 輸出：Mono                           │
   └─────────────────────────────────────┘
  ↓
⑨ Cornerstone Nucleo (Mono In/Stereo Out)
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • MODE: Reactor（核電廠模式）        │
   │ • DECAY: 60-90秒（極長）             │
   │ • BLEND: 50-80%                      │
   │ • FREEZE: 開啟（凍結音景）           │
   ├─────────────────────────────────────┤
   │ 目的：核電廠空間感 + 創造 Stereo     │
   │ 效果：建構複雜 Post Rock 音景        │
   │ 用法：                               │
   │ • AASB Shimmer → Nucleo 創造 Stereo  │
   │ • 雙 Freeze 建立底層音景             │
   │ 輸出：Stereo L+R                     │
   └─────────────────────────────────────┘
  ↓
⑩ Free the Tone FF-1Y Delay (Stereo In/Out)
   ┌─────────────────────────────────────┐
   │ 設定：                               │
   │ • MODE: Analog/Digital（視需求）     │
   │ • TIME: 長 Delay（1/2, 1/1 note）    │
   │ • FEEDBACK: 高（建構 Ambient Pad）   │
   │ • MIX: 40-70%                        │
   │ • HOLD: 開啟（建構音景層次）         │
   ├─────────────────────────────────────┤
   │ 目的：                               │
   │ 1. 精準 BPM 同步                     │
   │ 2. Hold 功能建構 Pad                 │
   │ 3. 保留並增強前面的 Stereo 寬度      │
   │ 效果：Post Rock 音景層次             │
   │ 輸出：完整 Stereo L+R                │
   └─────────────────────────────────────┘
  ↓
Toneking FX Return (Stereo L+R)
  ↓
Toneking Preamp 最終混合
  ↓
Toneking XLR Output L/R (stereo)
  ↓
🎚️ Audio Interface XLR Input L/R
```

### 效果器使用統計

| 效果器 | 使用率 | 角色 |
|--------|--------|------|
| PA-1QG | 95% | EQ 調整 |
| Cali76 FET | 80% | 染色壓縮 + Sustain |
| Roshi Blacklon | 75% | 管機模擬 |
| Morning Glory | 85% | Bluesbreaker OD |
| TWA Source Code | 60% | TS 中頻（Classic Rock 時） |
| ODL-1-CS | 70% | Dumble 高階音色 |
| AASB | 50% | Shimmer/Drone 底層 |
| Nucleo | 95% | 主 Reverb + 創造 Stereo |
| FF-1Y | 100% | 主 Delay + Hold + 增強 Stereo |

**總計**：9顆效果器（前級6顆 + 空間系3顆）

---

## 與 V3.0 (JC-22 版本) 對比分析

### 核心變更總結

| 項目 | V3.0 (JC-22) | Toneking Only | 變更說明 |
|------|--------------|---------------|----------|
| **音箱配置** | JC-22 + Toneking | 只有 Toneking | 移除 JC-22 |
| **效果器數量** | 12顆 | 14顆 | +2顆（CE-2W + Buffer++） |
| **Chorus** | JC-22 內建 | Boss CE-2W | 外部效果器替代 |
| **訊號鏈切換** | 兩台音箱 | Buffer++ Loop 切換 | 用路由器切換 |
| **錄音輸出** | Line Out | Stereo XLR | 專業級提升 |

### 訊號鏈1變更（Clean/Jazz/Neo Soul）

**V3.0 (JC-22)**：
```
Empress MKII → PA-1QG → Sweet Honey → Horsemeat → JC-22 Input
→ JC-22 Preamp (Chorus ON)
→ JC-22 FX Loop [FF-1Y, Nucleo]
→ JC-22 Output
```

**Toneking Only**：
```
PA-1QG → Buffer++ Loop 1 [Empress MKII, Sweet Honey, Horsemeat, CE-2W]
→ Toneking Rhythm Channel
→ Toneking FX Loop [AASB, Nucleo, FF-1Y]
→ Toneking XLR L/R → Interface
```

**改進**：
- ✅ **新增 CE-2W Chorus**：外部效果器完全替代 JC-22 Chorus
- ✅ **Stereo XLR 錄音**：專業級輸出，直接到 Interface
- ✅ **Buffer++ 切換**：腳踏即時切換，無需換音箱
- ⚠️ **Clean Tone 稍溫暖**：Toneking Rhythm Channel 是管機，比 JC-22 稍溫暖

### 訊號鏈2變更（Rock/Fusion/Post Rock）

**V3.0 (JC-22 或 Toneking)**：
```
Cali76 FET → PA-1QG → Blacklon → Morning Glory → Source Code → ODL-1-CS
→ 音箱 Input (JC-22 或 Toneking)
→ 音箱 FX Loop [FF-1Y, AASB, Nucleo]
→ 音箱 Output
```

**Toneking Only**：
```
PA-1QG → Buffer++ Loop 2 [Cali76 FET, Blacklon, Morning Glory, Source Code, ODL-1-CS]
→ Toneking Lead Channel
→ Toneking FX Loop [AASB, Nucleo, FF-1Y]
→ Toneking XLR L/R → Interface
```

**改進**：
- ✅ **統一使用 Toneking**：不需要切換音箱
- ✅ **Lead Channel 增益**：管機 overdrive 疊加前級 OD
- ✅ **Stereo XLR 錄音**：專業級輸出

---

## 豐富度對比評估

### 音色品質評分

| 評估項目 | V3.0 (JC-22) | Toneking Only | 說明 |
|---------|--------------|---------------|------|
| **Clean Tone 透明性** | ★★★★★ (98) | ★★★★☆ (90) | Toneking 稍溫暖 |
| **Chorus 效果** | ★★★★★ (95) | ★★★★★ (95) | CE-2W 完全替代 |
| **Stereo 空間感** | ★★★★★ (95) | ★★★★★ (98) | XLR 錄音更好 |
| **Rock/Fusion 音色** | ★★★★★ (96) | ★★★★★ (96) | 相同品質 |
| **錄音能力** | ★★★☆☆ (80) | ★★★★★ (98) | **顯著提升** |
| **訊號鏈彈性** | ★★★★☆ (85) | ★★★★★ (95) | Buffer++ 更便利 |
| **MIDI 控制** | ★★★★☆ (85) | ★★★★★ (98) | 完整 MIDI 系統 |
| **整體音色豐富度** | ★★★★★ (95) | ★★★★☆ (93) | 幾乎相同 |

### 優勢分析

#### ✅ Toneking Only 的優勢

1. **專業錄音能力提升**
   - Stereo XLR Outputs (L/R)
   - 直接輸出到 Audio Interface
   - 平衡訊號，低噪音
   - 不需要 DI Box

2. **訊號鏈切換更便利**
   - Buffer++ 腳踏切換
   - 無需換音箱
   - 即時響應

3. **完整 MIDI 控制**
   - PA-1QG 99 Preset
   - ODL-1-CS MIDI 控制
   - MOD 2 V2 統一管理

4. **管機音色選項**
   - Rhythm Channel (Clean)
   - Lead Channel (Overdrive)
   - 3 x 12AX7 tubes 真空管處理

5. **簡化設備**
   - 只需要一台 Preamp Pedal
   - 不需要兩台音箱
   - 便於移動和設置

#### ⚠️ Toneking Only 的妥協

1. **Clean Tone 不如 JC-22 透明**
   - Toneking Rhythm Channel 是管機
   - 比 JC-22 晶體機稍微溫暖
   - 但仍然是高品質 Clean Tone

2. **需要購買 Chorus 效果器**
   - 新增 Boss CE-2W ($180-200)
   - 佔用 1 個效果器位置
   - 但音色品質相當

3. **主 Pedalboard 增加 1 顆效果器**
   - 從 10 顆變成 11 顆
   - 需要稍大的 pedalboard

4. **沒有 JC-22 的 Stereo Speakers**
   - 錄音時沒問題（用 XLR）
   - 但練習/演出時需要監聽音箱或耳機

---

## 財務分析

### 賣出 JC-22 + 新增設備

| 項目 | 金額 | 說明 |
|------|------|------|
| **賣出 JC-22** | +$500-600 | 二手市場價格 |
| **購買 Boss CE-2W** | -$180-200 | Chorus 效果器 |
| **購買 Empress Buffer++** | -$299 | 訊號路由器 |
| **購買 Rockboard MOD 2 V2** | -$150-180 | Patchbay + MIDI |
| **淨支出** | **-$130-180** | 實際額外花費 |

**結論**：賣出 JC-22 後，額外支出約 **$130-180 USD** 即可完成轉換。

### 設備總價值

**主 Pedalboard 效果器**：
- PA-1QG: $425
- Buffer++: $299
- Empress MKII: $219
- Sweet Honey: $220
- Horsemeat: ~$150 (預估)
- CE-2W: $180-200
- Cali76 FET: $369
- Blacklon: $200
- Morning Glory: ~$150-180
- Source Code: $299
- ODL-1-CS: $425
- **主 pedalboard 總計**: **~$2,736-2,786**

**空間系 Pedalboard 效果器**：
- FF-1Y: $400
- AASB: $225
- Nucleo: $350
- **空間系總計**: **$975**

**Preamp & 配件**：
- Tone King Imperial MKII: $599
- MOD 2 V2: $150-180
- **總計**: **$749-779**

**整體系統總價值**：約 **$4,460-4,540 USD**

---

## 實施建議

### 階段1：準備新設備

**購買清單**：
1. ✅ Boss CE-2W Waza Craft Chorus ($180-200)
2. ✅ Empress Buffer++ ($299)
3. ✅ Rockboard MOD 2 V2 ($150-180)

**總支出**：約 $630-680 USD

### 階段2：訊號鏈組裝

**主 Pedalboard 配置（Loop 1 + Loop 2）**：
```
頂層（從左到右）：
① PA-1QG

中層（從左到右）：
② Buffer++ ③ Empress MKII ④ Sweet Honey ⑤ Horsemeat ⑥ CE-2W

底層（從左到右）：
⑦ Cali76 FET ⑧ Blacklon ⑨ Morning Glory ⑩ Source Code ⑪ ODL-1-CS
```

**空間系 Pedalboard 配置**：
```
獨立放置（從左到右）：
① AASB ② Nucleo ③ FF-1Y
```

### 階段3：接線配置

**主 Pedalboard 接線**：
```
吉他 → MOD 2 V2 TRS 1 → PA-1QG Input

PA-1QG Output → Buffer++ Input

Buffer++ Loop 1 Send → Empress MKII
Empress MKII → Sweet Honey → Horsemeat → CE-2W
CE-2W Output → Buffer++ Loop 1 Return

Buffer++ Loop 2 Send → Cali76 FET
Cali76 FET → Blacklon → Morning Glory → Source Code → ODL-1-CS
ODL-1-CS Output → Buffer++ Loop 2 Return

Buffer++ Output → MOD 2 V2 TRS 2 → Toneking Input
```

**MIDI 接線**：
```
MIDI Controller → MOD 2 V2 MIDI 1 → PA-1QG MIDI In
PA-1QG MIDI Thru → MOD 2 V2 MIDI 2 → ODL-1-CS MIDI In
```

**Toneking → 空間系 Pedalboard**：
```
Toneking FX Send → 空間系 pedalboard Input (AASB)
AASB Output → Nucleo Input
Nucleo Output L → FF-1Y Input L
Nucleo Output R → FF-1Y Input R
FF-1Y Output L → Toneking FX Return L
FF-1Y Output R → Toneking FX Return R
```

**Toneking → Interface**：
```
Toneking XLR Output L → Interface XLR Input L
Toneking XLR Output R → Interface XLR Input R
```

### 階段4：賣出 JC-22

**時機**：
- 完成新訊號鏈組裝後
- 測試確認音色滿意後

**預期售價**：$500-600 USD（二手市場）

**淨回收**：$500-600 - ($130-180 新設備淨支出) = **$320-470 USD 回收**

### 階段5：調整與優化

**Buffer++ 設定**：
- 設定為 Mode 5: Loop Select
- 分配腳踏開關：Loop 1 ↔ Loop 2 切換

**Toneking 設定**：
- Rhythm Channel: Clean Tone 設定
- Lead Channel: Overdrive 設定
- MIDI 通道設定（如需要）

**空間系效果器**：
- 確認 Stereo 連接正確
- 調整 Mix/Blend 比例
- 測試 Freeze 功能

---

## 使用建議

### Loop 1 (Clean/Jazz/Neo Soul) 使用場景

**最適合**：
- Jazz 演奏（Clean Tone + 微量 OD）
- Neo Soul 節奏（Sweet Honey + CE-2W Chorus）
- Funk Spank（Horsemeat Boost + Bright）
- Pop Rock（全部開啟）

**設定組合**：
- **極簡 Clean**：只開 PA-1QG + CE-2W
- **溫暖 Clean**：PA-1QG + Empress MKII + CE-2W
- **Neo Soul OD**：PA-1QG + Empress MKII + Sweet Honey + CE-2W
- **Solo Boost**：全部開啟 + Horsemeat

### Loop 2 (Rock/Fusion/Post Rock) 使用場景

**最適合**：
- Post Rock（高增益 + 複雜音景）
- Fusion（Dumble 音色 + 精準 Delay）
- Classic Rock（TS 中頻 + BB OD）
- Ambient（極長 Reverb + Shimmer）

**設定組合**：
- **Post Rock Crunch**：Cali76 + Blacklon (6L6) + Morning Glory
- **Fusion Clean OD**：Cali76 + ODL-1-CS (JAZZ Mode)
- **Classic Rock**：Blacklon + Morning Glory + Source Code
- **Ambient Pad**：全部開啟 + AASB Freeze → Nucleo Freeze → FF-1Y Hold
  （順序：Shimmer 底層 → Stereo Reverb → Stereo Delay 層次）

### Toneking 通道切換建議

**Rhythm Channel (Clean)**：
- Loop 1 使用
- MID-BITE: OFF
- VOLUME: 12-1點鐘
- 目的：保持清晰透明

**Lead Channel (Overdrive)**：
- Loop 2 使用
- MID-BITE: ON
- GAIN: 10-12點鐘
- 目的：疊加前級 OD，增加厚度

**切換方式**：
- 可用 Toneking 的 MIDI 或 Footswitch 切換
- 或保持固定通道，用 Buffer++ 切換 Loop

---

## 總結

### 核心優勢

1. **✅ 保留 90%+ 原本音色豐富度**
   - CE-2W 完全替代 JC-22 Chorus
   - Toneking Stereo FX Loop 保留 Stereo 能力
   - 管機 Clean Tone 僅稍微溫暖

2. **✅ 錄音能力顯著提升**
   - Stereo XLR Outputs 直接到 Interface
   - 專業級平衡訊號
   - 無需 DI Box

3. **✅ 訊號鏈切換更便利**
   - Buffer++ 腳踏切換
   - 即時響應，無延遲

4. **✅ 簡化設備配置**
   - 只需一台 Preamp Pedal
   - 便於移動和設置

5. **✅ 財務成本低**
   - 賣出 JC-22 後，淨支出僅 $130-180 USD
   - 甚至可能回收 $320-470 USD

6. **✅ 優化的空間系順序**
   - AASB → Nucleo → FF-1Y
   - 從 Mono 逐漸展開為完整 Stereo
   - Reverb → Delay 順序建構豐富音景層次
   - 最大化 Stereo 錄音品質

### 適合對象

**強烈推薦如果**：
- ✅ 你主要用途是錄音
- ✅ 你需要 Stereo XLR 輸出到 Interface
- ✅ 你想簡化設備（不需要兩台音箱）
- ✅ 你可以接受管機 Clean Tone（稍溫暖）
- ✅ 你願意購買 CE-2W Chorus 效果器

**不推薦如果**：
- ❌ 你非常依賴 JC-22 的晶體機透明性
- ❌ 你頻繁需要音箱 Stereo Speakers（演出/練習）
- ❌ 你不想增加效果器數量

### 最終建議

**這個配置可以完全保留原本訊號鏈的豐富度，並在以下方面有所提升**：

1. **錄音能力** - Stereo XLR 專業輸出
2. **訊號鏈彈性** - Buffer++ 即時切換
3. **MIDI 控制** - 完整的 MIDI 系統
4. **設備簡化** - 單一 Preamp Pedal
5. **空間系優化** - AASB → Nucleo → FF-1Y 最大化 Stereo 寬度

唯一的妥協是 Clean Tone 稍微不如 JC-22 透明，但 Toneking Rhythm Channel 仍然提供高品質的管機 Clean Tone，並且通過 CE-2W Chorus 可以完全重現 Neo Soul 的經典音色。

**整體評分**：★★★★☆ (93/100)

---

## 附錄

### 推薦線材

**TRS 訊號線**：
- 主 Pedalboard 內部跳線：短線 (15-30cm)
- 吉他到 pedalboard：3m
- Pedalboard 到 Toneking：1.5m
- Toneking 到空間系 pedalboard：依距離

**XLR 線**：
- Toneking 到 Interface：2 條 (L/R)，3-5m

**MIDI 線**：
- MIDI Controller 到 MOD 2 V2：3m
- MOD 2 V2 到 PA-1QG：1m
- PA-1QG 到 ODL-1-CS：1m

### 參考資料

- Tone King Imperial MKII 規格：shared/equipment_database/amps/tone_king_imperial_mkii.yaml
- Empress Buffer++ 規格：shared/equipment_database/pedals/empress_buffer_plus_plus.yaml
- Rockboard MOD 2 V2 規格：shared/equipment_database/accessories/rockboard_mod2_v2.yaml
- V3.0 訊號鏈參考：projects/2025-v3-signal-chain/signal_chains/signal_chain_v3.md

---

**文件版本**：Toneking Only v1.0
**最後更新**：2026-01-08
**狀態**：完整規劃，待實施測試
