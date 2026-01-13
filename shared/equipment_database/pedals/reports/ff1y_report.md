# Free the Tone FF-1Y FUTURE FACTORY - 器材詳細報告

**版本:** 1.0
**更新日期:** 2026-01-13
**資料來源:** `shared/equipment_database/pedals/specs/ff1y.yaml` + `pedals/examples/ff1y_examples.md`

---

## 目錄

1. [器材概述](#器材概述)
2. [技術規格詳解](#技術規格詳解)
3. [音色特性](#音色特性)
4. [使用範例](#使用範例)
5. [優缺點分析](#優缺點分析)
6. [網路驗證資訊](#網路驗證資訊)

---

## 器材概述

### 基本資訊

**品牌:** Free the Tone
**型號:** FF-1Y FUTURE FACTORY
**全名:** Free the Tone FUTURE FACTORY FF-1Y Digital Delay
**類型:** 數位雙延遲模組 Delay
**設計國:** 日本
**DSP:** 32-bit High-Precision DSP
**預設數量:** 128 個
**價格:** High-End Digital Delay 等級 (估計 $400-500 USD)

### 核心賣點

Free the Tone FF-1Y FUTURE FACTORY 是一款革命性的**雙延遲模組數位 Delay**，搭載世界首創的 **Random Fluctuating Phase Modulation** (隨機相位調變) 技術。不同於傳統 Delay 使用固定 LFO 調變，FF-1Y 的相位變化是**隨機產生**，創造更有機、更自然的「會呼吸」空間感。

這款效果器提供**雙延遲模組** (Delay A 和 Delay B)，可配置為**並聯 (Parallel)** 或**串聯 (Series)**，創造從簡單立體聲延遲到複雜疊加效果的極端音色範圍。搭配 **3-band EQ** (專用於塑造延遲音色)、**Soft Clipping Circuit** (添加類比溫暖感) 以及 **128 個預設槽位**，FF-1Y 成為 Free the Tone FUTURE FACTORY 系列的旗艦 Delay 產品。

**獨特之處:**
- **世界首創 Random Fluctuating Phase Modulation** - 隨機相位變化創造有機空間感
- **雙延遲模組** - 可獨立控制 Delay A 和 Delay B
- **串聯/並聯路由選擇** - 創造複雜延遲效果
- **3-band EQ** - 專用於塑造延遲音色，不影響原始訊號
- **Soft Clipping Circuit** - 為延遲訊號添加諧波，創造類比感
- **128 個預設** - 適合複雜現場演出或錄音室使用
- **MIDI 支援** - 整合外部控制器
- **Tap Tempo** - 節奏輸入快速配合歌曲 BPM
- **立體聲 I/O** - 雙輸入/雙輸出配置
- **Trail Function** - 切換預設時保留前一個延遲音
- **Phase Invert** - 反轉延遲音相位，解決頻率掩蓋問題
- **32-bit DSP** - 高音質處理
- **Built-in HTS Circuit** - 保持音色一致性

### 適合的音樂風格

| 風格 | 適配度 | 說明 |
|------|--------|------|
| **Post Rock** | ⭐⭐⭐⭐⭐ | 並聯模式創造豐富立體聲延遲層次 |
| **Ambient** | ⭐⭐⭐⭐⭐ | 長延遲 + Random Phase Modulation 創造無限音景 |
| **Jazz** | ⭐⭐⭐⭐⭐ | 細膩短延遲 (Slap Back) + 低 Mix |
| **Neo Soul** | ⭐⭐⭐⭐⭐ | 雙重延遲紋理增加厚度 |
| **Fusion** | ⭐⭐⭐⭐⭐ | 清晰延遲音質 + 動態響應 |
| **Math Rock** | ⭐⭐⭐⭐⭐ | 串聯模式創造節奏瀑布效果 |
| **Progressive Rock** | ⭐⭐⭐⭐⭐ | 複雜延遲設定 + 128 預設 |
| **Blues** | ⭐⭐⭐⭐ | Tape Echo 模擬 (Soft Clipping) |

**代表性應用場景:**
- Post Rock Ambient Layers
- Jazz Subtle Delays (Slap Back)
- Math Rock 複雜節奏分割
- Ambient 無限音景創造
- U2-style Dotted Eighth Note Delay

---

## 技術規格詳解

### 電源規格

| 項目 | 規格 | 說明 |
|------|------|------|
| **外部供電** | DC 9V | Center Negative |
| **電流消耗** | 350mA | **高電流需求** |
| **電池支援** | ❌ 不支援 | 需要穩定外部供電 |
| **Power Supply 需求** | **至少 400mA** | 建議使用獨立供電 |

**⚠️ 重要提示:**
- FF-1Y 電流消耗高達 350mA，需要至少 400mA 供電能力的 Power Supply
- 建議使用獨立輸出避免與其他效果器共用電源

---

### 尺寸與重量

- **尺寸:** 145.4mm (W) × 120.5mm (D) × 60mm (H)
- **重量:** 470g (約)

---

### DSP 架構

**處理器:** 32-bit High-Precision DSP
**訊號路徑:**
- **乾訊號:** 全類比 (Analog Dry Path)
- **延遲訊號:** 數位處理 (32-bit DSP)
- **混音:** 內部類比混音 (Built-in HTS Circuit)

**優勢:**
- 32-bit DSP 提供極高音質
- Analog Dry Path 保持原始訊號完整性
- HTS Circuit 確保效果開關時音色一致

---

### 雙延遲模組架構

#### **Dual Delay Units**

FF-1Y 搭載**兩組完全獨立的延遲模組** (Delay A 和 Delay B)，每組都有獨立的控制參數:

**Delay A / Delay B 各自控制:**
1. **Delay Time** - 延遲時間 (20ms ~ 2000ms，待手冊確認)
2. **Feedback** - 回授/重複次數 (0% ~ 無限重複)
3. **獨立 EQ** - 各自可調整 3-band EQ

---

#### **路由選擇: Parallel vs Series**

##### **Parallel Mode (並聯模式)**

**訊號流向:**
```
輸入訊號 ─┬─→ Delay A ─┬─→ 輸出
          └─→ Delay B ─┘
```

**特性:**
- 原始訊號**同時**送入兩組延遲
- 兩組延遲**獨立處理**後混合輸出
- 創造**豐富的立體聲效果**

**應用:**
- 立體聲 Ping-Pong Delay
- 雙重延遲紋理 (短 Slap Back + 長延遲)
- 寬廣立體聲空間感

---

##### **Series Mode (串聯模式)**

**訊號流向:**
```
輸入訊號 ─→ Delay A ─→ Delay B ─→ 輸出
```

**特性:**
- 訊號**先經過 Delay A**
- Delay A 的輸出**再送入 Delay B**
- 創造**疊加的複雜延遲效果**

**應用:**
- 節奏瀑布延遲 (Rhythmic Cascading)
- Tape Echo 模擬 (磁帶損耗)
- 複雜的延遲層次堆疊

---

### Random Fluctuating Phase Modulation (世界首創)

#### **傳統 Delay 調變 vs Random Phase Modulation**

**傳統 Delay 調變:**
- 使用固定 LFO (Low-Frequency Oscillator)
- 相位變化規律、可預測
- 調變音色較機械、人工

**Random Phase Modulation (FF-1Y):**
- 相位在訊號達到特定衰減水平時**隨機改變**
- 非固定週期，創造更有機感
- 延遲音「會呼吸」、自然飄浮

#### **調變控制**

**Modulation Depth (調變深度):**
- **低設定 (10-20%):** 細微的空間感增強，不明顯但豐富
- **中設定 (30-50%):** 明顯的調變效果，類比感
- **高設定 (60%+):** 極端調變，實驗性音色

**Modulation Rate (調變速率):**
- 待手冊確認 (可能與 Depth 連動或獨立控制)

---

### 3-Band EQ (延遲音色塑造)

**功能:**
- **僅塑造延遲音的音色，不影響原始訊號**
- Delay A 和 Delay B 各有獨立 EQ

**頻段:**
- **Low (低頻):** 待手冊確認 (典型為 100-200Hz)
- **Mid (中頻):** 待手冊確認 (典型為 800-1.5kHz)
- **High (高頻):** 待手冊確認 (典型為 3.2-6.4kHz)

**應用範例:**

| 音色需求 | Low | Mid | High | 效果 |
|---------|-----|-----|------|------|
| **清晰延遲** | -2dB | +1dB | +2dB | 明亮、清晰、現代感 |
| **溫暖延遲** | +2dB | 0dB | -3dB | 溫暖、類比感 |
| **背景 Pad 感** | -3dB | -2dB | -4dB | 延遲音融入背景 |
| **Tape Echo 模擬** | 0dB | 0dB | -2dB (Delay A) → -4dB (Delay B) | 磁帶漸暗效果 |

---

### Soft Clipping Circuit

**功能:**
- 為延遲訊號添加諧波內容
- 創造溫暖的類比感

**調整影響:**
- **關閉 (0%)** → 清晰的數位延遲音
- **開啟 (10-30%)** → 延遲音帶有溫暖的類比感
- **高設定 (40%+)** → 明顯的諧波豐富度，類似類比磁帶

**應用:**
- 數位清晰感: 關閉
- 類比溫暖感: 10-20%
- 磁帶回音模擬: 30-40%

---

### 控制旋鈕詳解

#### **主要旋鈕**

1. **Delay Time (×2)** - Delay A 和 Delay B 各一個
   - **功能:** 設定延遲音重複的時間間隔
   - **範圍:** 20ms ~ 2000ms (待手冊確認)
   - **短延遲 (20-120ms):** Slap Back、增加厚度
   - **中延遲 (120-400ms):** 節奏延遲、配合歌曲速度
   - **長延遲 (400ms+):** Ambient、音景創造

2. **Feedback (×2)** - Delay A 和 Delay B 各一個
   - **功能:** 控制延遲音重複的次數
   - **範圍:** 0% ~ 無限重複 (自我振盪)
   - **低 Feedback (1-2 次):** Slap Back、Jazz 細膩延遲
   - **中 Feedback (3-5 次):** 標準延遲效果
   - **高 Feedback (6 次+):** Ambient、Post Rock 音牆

3. **Mix (乾濕混合)**
   - **功能:** 調整原始訊號與延遲訊號的比例
   - **範圍:** 0% ~ 100%
   - **20-30%:** 細膩的延遲效果 (Jazz、Neo Soul)
   - **50%:** 乾濕各半
   - **70%+:** 明顯的延遲效果 (Ambient)

4. **3-Band EQ (×2)** - Delay A 和 Delay B 各一組
   - **Low / Mid / High**
   - **功能:** 塑造延遲音色，不影響原始訊號

5. **Modulation Controls (調變控制)**
   - **Depth:** 調變深度
   - **Rate:** 調變速率 (待手冊確認)

6. **Routing Select (路由選擇)**
   - **Parallel (並聯)** / **Series (串聯)**

7. **Soft Clipping Control**
   - 控制延遲訊號的諧波失真量

---

### 特殊功能

#### **1. Tap Tempo (節奏輸入)**

**功能:**
- 透過踩踏節拍，延遲時間自動同步歌曲速度
- 按 2-4 次節拍，FF-1Y 自動計算並設定延遲時間

**應用:**
- 現場演出快速配合歌曲 BPM
- U2-style Dotted Eighth Note Delay 設定

**計算公式範例 (120 BPM):**
- 四分音符 = 60000ms ÷ 120 = 500ms
- 附點八分音符 = 60000ms ÷ 120 ÷ 2 × 1.5 = 375ms

---

#### **2. Trail Function (延遲音延續)**

**功能:**
- 切換預設時，前一個預設的延遲音自然消失 (不會突然中斷)

**模式:**
- **開啟:** 自然的效果切換
- **關閉:** 立即切換

**應用:**
- 現場演出段落轉換更自然
- Studio 錄音保持延遲尾音完整性

---

#### **3. Phase Invert (相位反轉)**

**功能:**
- 反轉延遲音的相位 (180° 相位翻轉)

**應用:**
- 解決延遲音在樂團 Mix 中被其他樂器掩蓋的問題
- 創造特殊的空間感與相位抵消效果 (實驗性)

---

#### **4. Preset System (預設系統)**

**機身預設:**
- **數量:** 1-4 (機身快速切換)

**MIDI 預設:**
- **數量:** 128 個
- **控制:** 透過 MIDI Program Change 調用

**應用:**
- 複雜現場演出 (每首歌不同設定)
- Studio 錄音快速切換音色

---

### 連接規格

| 連接埠 | 規格 | 說明 |
|--------|------|------|
| **INPUT A** | 1/4" Phone Jack | 立體聲輸入 (左) |
| **INPUT B** | 1/4" Phone Jack | 立體聲輸入 (右) |
| **OUTPUT A** | 1/4" Phone Jack | 立體聲輸出 (左) |
| **OUTPUT B** | 1/4" Phone Jack | 立體聲輸出 (右) |
| **EXT (Tap)** | 1/4" Phone Jack | 外部 Tap Tempo 踏板 |
| **MIDI IN** | DIN 5-pin | MIDI 輸入 |
| **DC 9V** | 2.1mm Jack | Center Negative, 350mA |

**阻抗規格:**
- **輸入阻抗:** min. 500kΩ (高阻抗)
- **輸出阻抗:** min. 10kΩ (低阻抗負載)

**最大輸入電平:**
- **Inst (樂器):** +3.5dBu
- **Line (線路):** +11dBu

**⚠️ 重要:**
- FF-1Y 支援**立體聲輸入/輸出** (雙輸入/雙輸出配置)
- 可接單聲道或立體聲訊號源

---

## 音色特性

### 核心音色特徵

1. **清晰、高保真、精準**
   - 32-bit DSP 處理創造錄音室級音質
   - Analog Dry Path 保持原始訊號完整性

2. **有機、會呼吸的空間感**
   - Random Fluctuating Phase Modulation 創造自然調變
   - 延遲音如同「會呼吸」般飄浮

3. **極度靈活的音色塑造**
   - 3-band EQ 精準塑造延遲音色
   - Soft Clipping 添加類比溫暖感

4. **複雜的延遲層次**
   - 雙延遲模組創造豐富紋理
   - 串聯/並聯路由提供極端音色範圍

---

### 並聯模式 vs 串聯模式音色差異

#### **Parallel Mode (並聯模式)**

**音色特性:**
- 清晰、分離的延遲音
- 寬廣的立體聲空間感
- 兩組延遲不互相影響

**適合:**
- 需要寬廣立體聲效果
- 清晰的延遲音
- Post Rock Ambient Layers

---

#### **Series Mode (串聯模式)**

**音色特性:**
- 複雜、疊加的延遲音
- 延遲音會再產生延遲，創造多層節奏
- 訊號經過兩次處理，累積特性

**適合:**
- 複雜節奏疊加
- 類比磁帶感 (損耗累積)
- Math Rock 節奏分割

---

### Random Phase Modulation 在不同模式的表現

#### **並聯模式 + Random Phase Modulation**

**效果:**
- 兩組延遲各自產生隨機相位變化
- 非常寬廣、有機、會呼吸的立體聲空間
- 適合 Ambient、Post Rock、Neo Soul

**建議設定:** Modulation Depth 30-50%

---

#### **串聯模式 + Random Phase Modulation**

**效果:**
- 相位變化累積疊加 (Delay A 的調變被 Delay B 再次調變)
- 更極端、更實驗性的調變效果
- 適合 Experimental、Drone、Shoegaze

**建議設定:** Modulation Depth 40-60%

---

## 使用範例

### 範例 1：立體聲 Ping-Pong Delay (Parallel Mode)

**音樂風格:** Post Rock, Ambient, Neo Soul
**適合吉他:** 任何吉他

**設定:**

| 參數 | Delay A | Delay B |
|------|---------|---------|
| **Time** | 400ms (四分音符) | 600ms (附點四分音符) |
| **Feedback** | 3 次重複 | 3 次重複 |
| **Pan/Output** | Left (左聲道) | Right (右聲道) |
| **EQ Low** | 0dB | 0dB |
| **EQ Mid** | 0dB | 0dB |
| **EQ High** | +1dB | +2dB (略亮) |

**全局設定:**
- **Mix:** 40-50%
- **Modulation Depth:** 低 (10-20%)
- **Soft Clipping:** 關閉或極低
- **Routing:** Parallel

**效果:**
- 延遲音在左右聲道交替出現 (Ping-Pong 效果)
- 創造寬廣的立體聲空間感
- Random Phase Modulation 讓延遲音有細微的相位變化

**訊號鏈位置:**
```
Guitar → Compressor → Overdrive (輕度) → FF-1Y (Parallel) → Reverb → Stereo Amp
```

---

### 範例 2：Jazz Double Delay Texture (Parallel Mode)

**音樂風格:** Jazz, Fusion
**適合吉他:** 任何吉他

**設定:**

| 參數 | Delay A (短延遲) | Delay B (長延遲) |
|------|-----------------|-----------------|
| **Time** | 120ms (Slap Back) | 380ms (中長延遲) |
| **Feedback** | 1 次 | 4 次 |
| **EQ Low** | -2dB (削減混濁) | 0dB |
| **EQ Mid** | 0dB | 0dB |
| **EQ High** | +1dB | -2dB (溫暖) |

**全局設定:**
- **Mix:** 30%
- **Modulation Depth:** 中等 (30%)
- **Soft Clipping:** 10-15%
- **Routing:** Parallel

**效果:**
- 短延遲 (Delay A) 增加厚度和存在感
- 長延遲 (Delay B) 創造空間深度
- 兩者疊加創造複雜的延遲紋理
- Soft Clipping 添加細微的類比溫暖感

**訊號鏈位置:**
```
Guitar → Compressor → FF-1Y (Parallel) → Clean Amp
```

---

### 範例 3：Rhythmic Cascading Delay (Series Mode)

**音樂風格:** Math Rock, Progressive Rock
**適合吉他:** 任何吉他

**設定:**

| 參數 | Delay A | Delay B |
|------|---------|---------|
| **Time** | 200ms (十六分音符) | 400ms (八分音符) |
| **Feedback** | 2 次 | 3 次 |
| **EQ Low** | 0dB | 0dB |
| **EQ Mid** | +1dB | 0dB |
| **EQ High** | +2dB (保持清晰) | +1dB |

**全局設定:**
- **Mix:** 45%
- **Modulation Depth:** 低 (保持節奏精準)
- **Soft Clipping:** 關閉
- **Routing:** Series

**效果:**
```
原始音 → 200ms → 400ms → 600ms → 800ms → 1000ms...
```
- 創造多個節奏層次的疊加
- 形成類似「瀑布」般的延遲效果
- 每個重複音符都有自己的延遲鏈

**訊號鏈位置:**
```
Guitar → Overdrive → FF-1Y (Series) → Amp
```

---

### 範例 4：Tape Echo Emulation (Series Mode)

**音樂風格:** Blues, Classic Rock, Neo Soul
**適合吉他:** 任何吉他

**設定:**

| 參數 | Delay A (第一次損耗) | Delay B (第二次損耗) |
|------|-------------------|-------------------|
| **Time** | 350ms | 350ms (與 A 相同) |
| **Feedback** | 4 次 | 3 次 |
| **EQ Low** | 0dB | -1dB |
| **EQ Mid** | 0dB | -1dB |
| **EQ High** | -2dB (模擬磁帶損耗) | -4dB (再削減更多高頻) |

**全局設定:**
- **Mix:** 35%
- **Modulation Depth:** 中等 (30-40%，模擬 Wow & Flutter)
- **Soft Clipping:** 35% (明顯類比感)
- **Routing:** Series

**效果:**
- 延遲音經過兩次處理，每次都損失高頻
- 創造類比磁帶回音的漸暗效果
- Modulation 模擬磁帶不穩定的音高飄移
- Soft Clipping 添加磁帶飽和感

**訊號鏈位置:**
```
Guitar → Overdrive → FF-1Y (Series, Tape Echo) → Amp
```

---

### 範例 5：U2-style Dotted Eighth Note Delay (Series Mode)

**音樂風格:** U2-style Delay, Pop Rock
**適合吉他:** Single-Coil 吉他

**設定 (假設 120 BPM):**

| 參數 | Delay A | Delay B |
|------|---------|---------|
| **Time** | 375ms (附點八分音符 @ 120 BPM) | 375ms (與 A 相同) |
| **Feedback** | 3 次 | 2 次 |
| **EQ Low** | -1dB | -2dB |
| **EQ Mid** | 0dB | 0dB |
| **EQ High** | +1dB | +2dB (增加清晰度) |

**全局設定:**
- **Mix:** 40%
- **Modulation Depth:** 極低 (5-10%，保持節奏精準)
- **Soft Clipping:** 關閉
- **Routing:** Series
- **使用 Tap Tempo** 快速配合歌曲 BPM

**效果:**
```
原始音 → 375ms → 750ms → 1125ms → 1500ms...
但 Delay B 讓每個重複音有自己的延遲鏈
```
- 創造更複雜的附點八分音符節奏紋理
- 每個延遲音有「雙重回音」效果
- 保持節奏精準 (低 Modulation)

**訊號鏈位置:**
```
Guitar → Clean Boost → FF-1Y (Series) → Reverb → Amp
```

---

### 範例 6：Ambient Stereo Wash (Parallel Mode)

**音樂風格:** Post Rock, Shoegaze, Ambient
**適合吉他:** 任何吉他

**設定:**

| 參數 | Delay A | Delay B |
|------|---------|---------|
| **Time** | 500ms | 750ms (不同節奏比例) |
| **Feedback** | 6 次 (長重複) | 5 次 |
| **EQ Low** | +1dB | +2dB |
| **EQ Mid** | -2dB (削減，讓延遲音退到背景) | -3dB |
| **EQ High** | +1dB | 0dB |

**全局設定:**
- **Mix:** 60-70%
- **Modulation Depth:** 高 (50-60%)
- **Soft Clipping:** 30% (明顯類比感)
- **Routing:** Parallel

**效果:**
- 兩組不同時間的延遲創造複雜節奏紋理
- Random Phase Modulation 高設定讓延遲音「會呼吸」
- Soft Clipping 添加溫暖諧波
- EQ 削減中頻讓延遲音像 Ambient Pad

**訊號鏈位置:**
```
Guitar → Overdrive → FF-1Y (Parallel, High Mod) → Reverb → Stereo Amp
```

---

## 優缺點分析

### 優點

1. **世界首創 Random Fluctuating Phase Modulation**
   - 創造有機、會呼吸的延遲音
   - 不同於傳統固定 LFO 調變

2. **雙延遲模組設計極度靈活**
   - 並聯/串聯路由選擇
   - 一台效果器實現兩台 Delay 的效果

3. **專用 3-band EQ 極為實用**
   - 精準塑造延遲音色而不影響原始訊號
   - Delay A 和 Delay B 各有獨立 EQ

4. **Soft Clipping 添加類比溫暖感**
   - 為數位延遲添加諧波豐富度
   - 可模擬 Tape Echo

5. **128 個預設 + MIDI 支援**
   - 適合複雜現場演出或錄音室使用
   - 3 個機身預設快速切換

6. **立體聲 I/O 支援**
   - 充分發揮雙音箱或立體聲 FX Loop 的能力
   - 並聯模式創造寬廣立體聲效果

7. **32-bit DSP 高音質處理**
   - 錄音室級延遲音質
   - Analog Dry Path 保持原始訊號完整性

8. **Trail Function 切換自然**
   - 切換預設時延遲音不會突然中斷
   - 現場演出更流暢

9. **Tap Tempo 支援**
   - 快速配合歌曲 BPM
   - 現場演出極為實用

10. **Phase Invert 功能**
    - 解決延遲音被掩蓋的問題
    - 創造特殊空間感

---

### 缺點

1. **價格較高**
   - 估計 $400-500 USD
   - 屬於 High-End Digital Delay 等級

2. **電流需求高**
   - 350mA 電流消耗
   - 需要至少 400mA 供電能力

3. **體積較大**
   - 145.4 × 120.5mm
   - Pedalboard 空間佔用較多

4. **學習曲線較陡**
   - 雙延遲模組 + 多種功能需要時間熟悉
   - 不適合希望即插即用的玩家

5. **複雜功能可能過度**
   - 對只需要簡單延遲的玩家可能過於複雜
   - 部分功能 (如 Phase Invert) 較少使用

6. **不支援電池**
   - 需要穩定外部供電
   - 無法使用電池供電

---

### 適合人群

**最適合:**
- Post Rock, Ambient, Math Rock 玩家
- Jazz/Fusion 玩家 (追求細膩延遲音質)
- 追求錄音室級延遲音質的專業音樂家
- 需要複雜延遲設定的玩家
- MIDI 整合系統使用者
- 追求創意延遲效果的實驗性玩家
- 需要立體聲延遲效果的玩家

**較不適合:**
- 預算有限的初學者
- 追求簡單、即插即用的玩家
- Pedalboard 空間極度有限的玩家
- 只需要基本延遲功能的玩家
- 追求類比 Delay 音色的玩家 (考慮真實 Analog Delay)

---

## 網路驗證資訊

### 驗證來源

本報告的關鍵資訊已透過以下來源驗證:

1. **[Free the Tone 官方產品頁面](https://www.freethetone.com/en/products/detail43/)**
   - 完整技術規格
   - 官方產品描述

2. **[MusicRadar 評測](https://www.musicradar.com/reviews/free-the-tone-future-factory-ff-1y-delay)**
   - 專業評測與音色分析
   - 「非常多功能的踏板，處理所有標準延遲任務，並專精於調變與延遲結合創造獨特 ambience」

3. **[Reverb 產品頁面](https://reverb.com/p/free-the-tone-ff-1y-future-factory-rf-phase-modulation-delay)**
   - 市場價格
   - 用戶評價

4. **[Pedal of the Day 報導](https://www.pedal-of-the-day.com/2019/04/09/free-the-tone-future-factory-ff-1y-rf-phase-modulation-delay/)**
   - 產品特色介紹

5. **[Guitars Rebellion 評論](https://www.guitarsrebellion.com/en/products/free-the-tone-future-factory-ff-1y)**
   - 「巨大的空間化效果，獨特的 3D 深度與美妙的調變」

### 驗證的關鍵資訊

- ✅ 世界首創 Random Fluctuating Phase Modulation
- ✅ 雙延遲模組 (Delay A 和 Delay B)
- ✅ 串聯/並聯路由選擇
- ✅ 3-band EQ 專用於塑造延遲音色
- ✅ Soft Clipping Circuit
- ✅ 128 個預設槽位
- ✅ 32-bit High-Precision DSP
- ✅ Built-in HTS Circuit
- ✅ Tap Tempo 支援
- ✅ MIDI 支援 (DIN 5-pin)
- ✅ Trail Function
- ✅ Phase Invert
- ✅ 立體聲 I/O (雙輸入/雙輸出)
- ✅ 輸入阻抗 min. 500kΩ
- ✅ 輸出阻抗 min. 10kΩ
- ✅ 電源 9V DC, 350mA
- ✅ 尺寸 145.4 × 120.5 × 60mm, 470g

### 評測摘要

**MusicRadar:**
> "A very versatile pedal that will take care of all standard delay duties but specialises in composite sounds where modulation and delay combine to create unique ambiences."
> (非常多功能的踏板，處理所有標準延遲任務，並專精於調變與延遲結合創造獨特 ambience。)

**Guitars Rebellion:**
> "Enormous spatialization with a kind of unique 3D depth with a wonderful modulation."
> (巨大的空間化效果，獨特的 3D 深度與美妙的調變。)

---

## 總結

### 核心優勢

Free the Tone FF-1Y FUTURE FACTORY 是一款革命性的雙延遲模組數位 Delay，搭載世界首創的 **Random Fluctuating Phase Modulation** 技術，創造有機、會呼吸的延遲音。**雙延遲模組** (並聯/串聯路由)、**專用 3-band EQ**、**Soft Clipping Circuit** 以及 **128 個預設** 讓這款效果器成為 Free the Tone FUTURE FACTORY 系列的旗艦產品。

32-bit DSP 提供錄音室級音質，Analog Dry Path 保持原始訊號完整性，立體聲 I/O 充分發揮雙音箱或立體聲 FX Loop 的能力。適合 Post Rock、Ambient、Jazz、Math Rock 等需要複雜延遲設定的音樂風格。

### 最佳使用建議

1. **初學者:** 從並聯模式開始，使用相近的 Delay Time，Mix 保持 30-40%
2. **中階使用者:** 實驗不同的 Delay Time 組合，善用 3-band EQ 塑造音色
3. **進階使用者:** 串聯模式 + Phase Invert + 極端 Modulation 創造實驗性音色，建立完整的 128 預設庫

### 模式選擇快速指南

| 需求 | 模式選擇 | 原因 |
|------|---------|------|
| 寬廣立體聲效果 | Parallel | 兩組延遲可分配左右聲道 |
| 複雜節奏疊加 | Series | 延遲音會再產生延遲 |
| 清晰的延遲音 | Parallel | 兩組延遲不互相影響 |
| 類比磁帶感 | Series | 訊號經過兩次處理，累積類比特性 |

### 訊號鏈定位

**最佳位置:** FX Loop 或 Post-Gain (Overdrive 之後)

**推薦配置 (Stereo):**
```
Guitar → Compressor → Overdrive → FF-1Y (Parallel/Series) → Reverb → Stereo Amp
```

**Ambient 配置:**
```
Guitar → Clean Boost → FF-1Y (High Modulation) → Reverb (Shimmer) → Stereo Amp
```

**Math Rock 配置:**
```
Guitar → Overdrive → FF-1Y (Series, Rhythmic Cascade) → Amp
```

---

**文件版本:** 1.0
**最後更新:** 2026-01-13
**下次更新計劃:** 補充實際手冊確認的旋鈕範圍與頻段參數

**相關文件:**
- `shared/equipment_database/pedals/specs/ff1y.yaml` - FF-1Y 完整技術規格
- `shared/equipment_database/pedals/examples/ff1y_examples.md` - FF-1Y 詳細使用範例與控制說明
- `projects/2025-v3-signal-chain/research/compressor_eq_spatial_effects_technical_data.md` - 空間系效果器技術資料

---

**參考資料來源:**
- [Free the Tone 官方產品頁面](https://www.freethetone.com/en/products/detail43/)
- [MusicRadar 評測](https://www.musicradar.com/reviews/free-the-tone-future-factory-ff-1y-delay)
- [Reverb 產品頁面](https://reverb.com/p/free-the-tone-ff-1y-future-factory-rf-phase-modulation-delay)
- [Pedal of the Day 報導](https://www.pedal-of-the-day.com/2019/04/09/free-the-tone-future-factory-ff-1y-rf-phase-modulation-delay/)
- [Guitars Rebellion 評論](https://www.guitarsrebellion.com/en/products/free-the-tone-future-factory-ff-1y)
