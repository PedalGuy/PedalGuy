# Free The Tone PA-1QG Programmable Analog 10 Band EQ - 器材詳細報告

**版本:** 1.0
**更新日期:** 2026-01-13
**資料來源:** `shared/equipment_database/pedals/specs/pa1qg.yaml`

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
**型號:** PA-1QG Programmable Analog 10 Band EQ
**類型:** EQ / Preamp
**風格:** Parametric & Graphic EQ
**設計師:** Yuki Hayashi
**製造國:** Japan
**發行年份:** 2018
**開發時間:** 10+ 年研發

### 核心賣點

Free the Tone PA-1QG 是一款結合**類比音質**與**數位便利**的革命性可程式化 EQ。這款由 Yuki Hayashi（Free the Tone 創辦人，同時也是 ODL-1-CS 設計師）耗時 10 年以上研發的效果器，於 2018 年 NAMM 展發表，被譽為「當時市場上最好的踏板格式 EQ」。

PA-1QG 最獨特之處在於：**全類比訊號路徑 + 數位參數控制**，提供 **99 組可程式化預設**，每組預設都有獨立的 10 頻段 EQ（±12dB）和獨立音量控制（0-127）。配合 Free the Tone 獨家的 **HTS Circuit**（Holistic Tonal Solution），確保效果開關時音色質感一致。

**獨特之處:**
- **99 組可程式化預設** - 為每把吉他、每種風格建立專用 EQ
- **全類比訊號路徑** - 高品質類比音色，無數位失真
- **10 頻段針對吉他優化** - 50Hz~10kHz，專為吉他音域設計
- **獨立音量控制** - 每預設獨立 LEVEL（0-127），可作 Preset-based Volume Controller
- **HTS Circuit** - 確保效果開關時音色質感一致
- **完整 MIDI 支援** - Program Change / Control Change

### 適合的音樂風格

| 風格 | 適配度 | 說明 |
|------|--------|------|
| **多吉他演奏者** | ⭐⭐⭐⭐⭐ | 為每把吉他建立專用 EQ 預設 |
| **現場演出** | ⭐⭐⭐⭐⭐ | 快速預設切換，適應不同曲目 |
| **Jazz** | ⭐⭐⭐⭐⭐ | 精確 EQ 塑形，調整音色平衡 |
| **Fusion** | ⭐⭐⭐⭐⭐ | 多種音色需求，快速切換 |
| **Studio Recording** | ⭐⭐⭐⭐⭐ | 精確 EQ 控制，類比音質 |
| **MIDI 整合系統** | ⭐⭐⭐⭐⭐ | 完整 MIDI 支援，系統整合 |

**代表性應用場景:**
- 多把吉他切換（每把吉他獨立 EQ）
- 現場演出快速預設切換
- Solo Boost（透過 LEVEL 設定）
- 不同曲風音色切換
- MIDI 整合系統

---

## 技術規格詳解

### 電源規格

| 項目 | 規格 | 說明 |
|------|------|------|
| **外部供電** | DC 9V | Center Negative |
| **電流消耗** | 200mA | **需要 200mA 以上供電能力** |
| **電池支援** | ❌ 不支援 | 高電流消耗，不適合電池供電 |

**⚠️ 重要提示:**
- 200mA 高電流消耗，**不建議 Daisy Chain**
- 建議使用獨立 Power Supply 輸出

---

### EQ 系統

**EQ 類型:** 10-Band Programmable Graphic EQ

**10 頻段（針對吉他優化）:**
1. **50Hz** - 極低頻（控制低頻基礎）
2. **100Hz** - 低頻（豐富度與厚度）
3. **200Hz** - 低中頻（Body 感）
4. **400Hz** - 中低頻（溫暖度）
5. **800Hz** - 中頻（存在感）
6. **1.5kHz** - 中高頻（清晰度）
7. **2.5kHz** - 高中頻（咬合感）
8. **3.5kHz** - 高頻（明亮度）
9. **7kHz** - 高頻（光澤感）
10. **10kHz** - 極高頻（空氣感）

**調整範圍:** ±12 dB per band

---

### 預設系統

**預設數量:** 99 組

**快速存取預設:** 1-4（前面板 PRESET 開關）
**MIDI 存取:** 全部 99 組可透過 MIDI 存取

**每組預設包含:**
- 10 頻段 EQ 設定（±12dB）
- 獨立音量控制（LEVEL: 0-127）
  - Unity Gain = 100
  - 最大 Boost = 127（+12dB）

---

### 控制介面

**旋轉編碼器:**
- **Cursor Keys** - 選擇頻段或 Volume
- **PARAMETER Encoder** - 調整選定參數

**開關:**
- **PRESET Switch** - 切換預設 1-4
- **ON/OFF Switch** - 效果開關
- **SAVE Switch** - 儲存預設

**顯示:**
- **EQ 曲線顯示** - 即時顯示 EQ 曲線
- **LEVEL 顯示** - 顯示音量設定

---

### MIDI 功能

**MIDI 支援:** 完整

**功能:**
- **Program Change** - 切換預設 1-99
- **Control Change** - 控制參數
- **MIDI Channel** - 可設定（ALL / 1-16 / OFF）

**應用場景:**
- MIDI Switcher 整合（如 RJM Mastermind）
- DAW 錄音自動化
- 現場演出 MIDI 控制

---

### HTS Circuit (Holistic Tonal Solution)

**特性:**
- 全面管理高品質訊號
- 解決傳統 Bypass 音色差異問題
- 確保效果開關時音色質感一致
- 輸出與輸入同相位

**Bypass 方式:** Buffered Bypass (Always-on)

---

### 阻抗特性

| 項目 | 規格 | 說明 |
|------|------|------|
| **輸入阻抗（INST）** | 1MΩ | 適合吉他被動拾音器 |
| **輸入阻抗（LINE）** | 300kΩ | 適合 Line Level 訊號 |
| **輸出阻抗** | min. 10kΩ | 適合驅動後級效果器 |
| **最大輸入（INST）** | +4dBu | 吉他輸入 |
| **最大輸入（LINE）** | +14dBu | Line 輸入 |

**⚠️ 注意:**
- 輸入阻抗可切換（INST / LINE）

---

## 音色特性

### 核心音色特徵

1. **類比音質優異**
   - 全類比訊號路徑
   - 無數位失真或延遲
   - 溫暖、自然的音色

2. **10 頻段針對吉他優化**
   - 50Hz~10kHz 涵蓋吉他音域
   - 頻段選擇科學，避免過度重疊
   - 適合吉他音色塑形

3. **HTS Circuit 確保訊號品質**
   - 效果開關時音色質感一致
   - 不同於傳統 Buffer
   - 最大化吉他音色特性

4. **透明但可塑性高**
   - 不改變基礎音色特性
   - 但可大幅調整頻率平衡（±12dB）

---

### 頻率調整建議

**增加溫暖度:**
- 提升 100Hz, 200Hz, 400Hz
- 略削減 3.5kHz, 7kHz

**增加明亮度:**
- 提升 2.5kHz, 3.5kHz, 7kHz
- 略削減 200Hz, 400Hz

**增加存在感:**
- 提升 800Hz, 1.5kHz, 2.5kHz

**削減冰冷感（Stratocaster）:**
- 削減 3.5kHz, 7kHz, 10kHz
- 提升 200Hz, 400Hz

**控制過多中頻（Les Paul）:**
- 削減 400Hz, 800Hz
- 提升 2.5kHz, 7kHz

---

### Clean Boost 功能

**透過 LEVEL 控制:**
- LEVEL = 100 → Unity Gain
- LEVEL = 110 → 輕微 Boost
- LEVEL = 127 → +12dB Boost

**應用場景:**
- Solo Boost（建立 Solo 專用預設，LEVEL 設定 120-127）
- 音量補償（不同吉他音量差異補償）
- 推動 Overdrive（Boost 功能）

---

## 使用範例

### 範例 1：Telecaster 專用 EQ（增加低頻與中頻）

**適合吉他:** Telecaster（Neck Pickup 較薄）
**預設編號:** Preset 1

**EQ 設定:**

| 頻段 | 調整 | 說明 |
|------|------|------|
| **50Hz** | 0dB | 保持平坦 |
| **100Hz** | +3dB | 增加低頻豐富度 |
| **200Hz** | +4dB | 增加 Body 感 |
| **400Hz** | +3dB | 增加溫暖度 |
| **800Hz** | +2dB | 增加存在感 |
| **1.5kHz** | 0dB | 保持平坦 |
| **2.5kHz** | +1dB | 略增咬合感 |
| **3.5kHz** | 0dB | 保持平坦 |
| **7kHz** | -2dB | 略削減冰冷感 |
| **10kHz** | -1dB | 略削減冰冷感 |

**LEVEL:** 100（Unity Gain）

**效果:**
- Telecaster Neck Pickup 不再單薄
- 增加低頻豐富度與中頻存在感
- 略削減 Tele 特有的冰冷感

**訊號鏈位置:** Guitar → Compressor → **PA-1QG (Preset 1)** → Overdrive → Amp

---

### 範例 2：Stratocaster 專用 EQ（削減冰冷感）

**適合吉他:** Stratocaster（Bridge Pickup 較亮）
**預設編號:** Preset 2

**EQ 設定:**

| 頻段 | 調整 | 說明 |
|------|------|------|
| **50Hz** | 0dB | 保持平坦 |
| **100Hz** | +2dB | 增加低頻 |
| **200Hz** | +3dB | 增加 Body 感 |
| **400Hz** | +2dB | 增加溫暖度 |
| **800Hz** | 0dB | 保持平坦 |
| **1.5kHz** | 0dB | 保持平坦 |
| **2.5kHz** | 0dB | 保持平坦 |
| **3.5kHz** | -3dB | 削減冰冷感 |
| **7kHz** | -4dB | 削減冰冷感 |
| **10kHz** | -2dB | 略削減極高頻 |

**LEVEL:** 100（Unity Gain）

**效果:**
- Stratocaster Bridge Pickup 不再刺耳
- 增加溫暖度，削減冰冷感
- 保留 Strat 特有的清晰度

**訊號鏈位置:** Guitar → Compressor → **PA-1QG (Preset 2)** → Overdrive → Amp

---

### 範例 3：Les Paul 專用 EQ（控制過多中頻）

**適合吉他:** Les Paul（Humbucker 中頻豐富）
**預設編號:** Preset 3

**EQ 設定:**

| 頻段 | 調整 | 說明 |
|------|------|------|
| **50Hz** | 0dB | 保持平坦 |
| **100Hz** | +1dB | 略增低頻 |
| **200Hz** | -2dB | 削減泥濘感 |
| **400Hz** | -3dB | 削減過多中頻 |
| **800Hz** | -2dB | 削減過多中頻 |
| **1.5kHz** | 0dB | 保持平坦 |
| **2.5kHz** | +2dB | 增加清晰度 |
| **3.5kHz** | +2dB | 增加明亮度 |
| **7kHz** | +3dB | 增加光澤感 |
| **10kHz** | +1dB | 略增空氣感 |

**LEVEL:** 100（Unity Gain）

**效果:**
- Les Paul Humbucker 不再過度中頻
- 削減泥濘感，增加清晰度
- 增加高頻光澤感

**訊號鏈位置:** Guitar → Compressor → **PA-1QG (Preset 3)** → Overdrive → Amp

---

### 範例 4：Hollowbody 專用 EQ（削減 Feedback 頻率）

**適合吉他:** Semi-Hollow / Hollowbody（容易 Feedback）
**預設編號:** Preset 4

**EQ 設定:**

| 頻段 | 調整 | 說明 |
|------|------|------|
| **50Hz** | -2dB | 削減極低頻 Feedback |
| **100Hz** | -3dB | 削減低頻 Feedback |
| **200Hz** | -4dB | 削減主要 Feedback 頻率 |
| **400Hz** | -2dB | 削減 Feedback |
| **800Hz** | 0dB | 保持平坦 |
| **1.5kHz** | +1dB | 增加清晰度 |
| **2.5kHz** | +2dB | 增加咬合感 |
| **3.5kHz** | +1dB | 增加明亮度 |
| **7kHz** | 0dB | 保持平坦 |
| **10kHz** | 0dB | 保持平坦 |

**LEVEL:** 100（Unity Gain）

**效果:**
- 大幅削減 Hollowbody 容易 Feedback 的頻率（100-400Hz）
- 增加中高頻清晰度
- 適合現場演出高音量

**訊號鏈位置:** Guitar → Compressor → **PA-1QG (Preset 4)** → Overdrive → Amp

---

### 範例 5：Solo Boost（音量提升 + EQ 塑形）

**適合風格:** 任何風格的 Lead Solo
**預設編號:** Preset 5

**EQ 設定:**

| 頻段 | 調整 | 說明 |
|------|------|------|
| **50Hz** | -2dB | 削減低頻（避免泥濘） |
| **100Hz** | -1dB | 削減低頻 |
| **200Hz** | 0dB | 保持平坦 |
| **400Hz** | +1dB | 略增溫暖度 |
| **800Hz** | +3dB | 增加存在感 |
| **1.5kHz** | +4dB | 增加清晰度 |
| **2.5kHz** | +5dB | 增加咬合感（Solo 穿透力） |
| **3.5kHz** | +3dB | 增加明亮度 |
| **7kHz** | +2dB | 增加光澤感 |
| **10kHz** | 0dB | 保持平坦 |

**LEVEL:** 120（+8dB Boost）

**效果:**
- +8dB 音量提升（Solo Boost）
- 增加中高頻存在感與穿透力
- 削減低頻避免與 Band 混濁
- 適合 Lead Solo 時開啟

**訊號鏈位置:** Guitar → Compressor → Overdrive → **PA-1QG (Preset 5)** → Delay → Amp

**應用場景:**
- Solo 時切換到 Preset 5
- 音量提升 + EQ 塑形一次完成
- 配合 Overdrive 使用，創造飽滿 Lead 音色

---

### 範例 6：Funk Rhythm（增加咬合感）

**適合風格:** Funk, R&B
**預設編號:** Preset 6

**EQ 設定:**

| 頻段 | 調整 | 說明 |
|------|------|------|
| **50Hz** | -3dB | 削減極低頻 |
| **100Hz** | -2dB | 削減低頻（避免糊） |
| **200Hz** | 0dB | 保持平坦 |
| **400Hz** | +1dB | 略增溫暖度 |
| **800Hz** | +2dB | 增加存在感 |
| **1.5kHz** | +3dB | 增加清晰度 |
| **2.5kHz** | +5dB | 增加 Funky 咬合感 |
| **3.5kHz** | +4dB | 增加明亮度 |
| **7kHz** | +2dB | 增加光澤感 |
| **10kHz** | +1dB | 略增空氣感 |

**LEVEL:** 105（+2dB 輕微 Boost）

**效果:**
- 大幅提升 2.5kHz 和 3.5kHz，增加 Funky 咬合感
- 削減低頻避免糊掉
- 輕微 Boost，增加存在感

**訊號鏈位置:** Guitar → Compressor → **PA-1QG (Preset 6)** → Amp

**搭配建議:**
- 配合 Compressor（快速 Attack/Release）使用
- 適合 Single-Coil 吉他（Stratocaster）

---

## 優缺點分析

### 優點 ✅

1. **類比音質優異**
   - 全類比訊號路徑
   - 無數位失真或延遲
   - 溫暖、自然的音色

2. **99 組預設充足**
   - 為每把吉他建立專用 EQ
   - 為每種風格建立專用設定
   - 現場演出快速切換

3. **HTS Circuit**
   - 確保效果開關時音色質感一致
   - 不同於傳統 Buffer
   - 最大化吉他音色特性

4. **MIDI 支援完整**
   - Program Change / Control Change
   - MIDI Channel 可設定
   - 適合 MIDI 整合系統

5. **可作 Volume Controller**
   - 每預設獨立 LEVEL（0-127）
   - 可作為 Preset-based Volume Controller
   - Solo Boost 功能

6. **10 頻段針對吉他優化**
   - 50Hz~10kHz 涵蓋吉他音域
   - 頻段選擇科學
   - ±12dB 調整範圍充足

7. **Buffered Output**
   - 低輸出阻抗，適合驅動後級效果器
   - 長線材使用不失真

---

### 缺點 ❌

1. **價格較高**
   - MSRP $425 USD
   - 屬於 High-End 等級

2. **學習曲線陡**
   - 需要理解 EQ 概念
   - 需要時間建立預設庫
   - 不適合即插即用

3. **需要時間建立預設庫**
   - 99 組預設需要逐一設定
   - 初期需要投入時間實驗
   - 但一旦建立完成，極度便利

4. **體積較大**
   - 相較於一般 EQ 踏板較大
   - Pedalboard 空間佔用較多

5. **高電流消耗**
   - 200mA 電流消耗
   - 不建議 Daisy Chain
   - 需要獨立 Power Supply 輸出

---

### 適合人群 🎯

**最適合:**
- 擁有多把吉他的玩家（為每把吉他建立專用 EQ）
- 現場演出玩家（快速預設切換）
- 需要多組 EQ 設定的玩家（不同風格/曲目）
- 追求類比音質的玩家
- MIDI 整合系統使用者
- 專業錄音應用
- 願意花時間深入研究的玩家

**較不適合:**
- 預算有限的初學者
- 只有一把吉他的玩家（可能用不到 99 組預設）
- 希望即插即用、不想調整的玩家
- 不理解 EQ 概念的玩家
- Pedalboard 空間極有限的玩家

---

## 網路驗證資訊

### 驗證來源

本報告的關鍵資訊已透過以下來源驗證：

1. **[Free the Tone 官方產品頁面](https://www.freethetone.com/en/products/detail18/)**
   - 完整技術規格
   - 官方設計理念說明

2. **[MusicRadar 評測（2018 年 8 月）](https://www.musicradar.com/reviews/free-the-tone-programmable-analog-eq)**
   - 專業評測與音色分析

3. **[Premier Guitar 報導（2018 年 1 月）](https://www.premierguitar.com/free-the-tone-unveils-programmable-analog-10-band-eq)**
   - 產品發表報導

4. **[Pedal of the Day（2018 年 2 月）](https://www.pedal-of-the-day.com/2018/02/09/free-tone-pa-1qg-programmable-analog-10-band-eq/)**
   - 詳細評測

5. **[The Gear Page 論壇討論](https://www.thegearpage.net/board/index.php?threads/free-the-tone-pa-1qg-eq-reviews.2139058/)**
   - 用戶評價

### 驗證的關鍵資訊 ✓

- ✅ 2018 年 NAMM 展發表
- ✅ 開發耗時 10+ 年
- ✅ 設計師 Yuki Hayashi（ODL-1-CS 同一設計師）
- ✅ 9V DC 200mA 供電
- ✅ 10 頻段：50Hz, 100Hz, 200Hz, 400Hz, 800Hz, 1.5kHz, 2.5kHz, 3.5kHz, 7kHz, 10kHz
- ✅ 調整範圍 ±12dB per band
- ✅ 99 組預設（1-4 快速存取，5-99 MIDI 存取）
- ✅ 每預設獨立 LEVEL（0-127）
- ✅ HTS Circuit（Holistic Tonal Solution）
- ✅ Buffered Bypass
- ✅ 完整 MIDI 支援
- ✅ 建議售價 $425 USD（2018 年發表時為 $380）

### 評測重點

**MusicRadar (2018 年 8 月):**
> "Sonically, the quality and level of control offered by the PA-1QG was superb: from adding a sparkle and spritz to muddy pickups to injecting juicy midrange to overdriven lead sounds"
>
> （音色上，PA-1QG 提供的品質和控制水準極為出色：從為渾濁的拾音器增加閃亮感，到為 Overdrive Lead 音色注入飽滿的中頻）

**Guitars Rebellion:**
> "The Free The Tone Programmable Analog 10 Band EQ is, at the time of writing, surely the best pedal format EQ available on the market."
>
> （Free The Tone Programmable Analog 10 Band EQ 在當時（2018），無疑是市場上最好的踏板格式 EQ）

**Pedal of the Day (2018 年 2 月):**
> "Another marvelous masterpiece from the Free The Tone crew, if you're looking to truly fine-tune your sound without sacrificing any tone to the evils of digital processing"
>
> （Free The Tone 團隊的另一個奇妙傑作，如果你想真正微調你的音色，又不想犧牲任何音色給數位處理的邪惡）

---

## 總結

### 核心優勢

Free the Tone PA-1QG 是市面上少數結合**類比音質**與**數位便利**的高階可程式化 EQ。Yuki Hayashi 耗時 10 年以上研發，全類比訊號路徑 + 數位參數控制，99 組可程式化預設，每組預設獨立的 10 頻段 EQ 和音量控制，配合 HTS Circuit 確保訊號品質，讓這款 EQ 成為多吉他演奏者、現場演出玩家、MIDI 整合系統使用者的終極選擇。

### 最佳使用建議

1. **初學者:** 從簡單的吉他專用 EQ 開始（範例 1-4），為每把吉他建立基礎 EQ 預設
2. **中階使用者:** 實驗不同風格的 EQ 設定（範例 5-6），建立風格專用預設
3. **進階使用者:** 建立完整的 99 組預設庫，配合 MIDI 系統整合，實現現場演出快速切換

### 預設策略建議

**建議預設分配:**
- **Preset 1-4:** 快速存取，常用音色（4 把主力吉他）
- **Preset 5-20:** 不同吉他專用 EQ（涵蓋所有吉他）
- **Preset 21-40:** 不同音樂風格（Jazz, Funk, Rock, Blues 等）
- **Preset 41-60:** Solo Boost 變化（不同 EQ + Level）
- **Preset 61-99:** 實驗與特殊用途

### 訊號鏈定位

**最佳位置:** Signal Chain 前段（Always-on Pre-Amp）

**推薦配置:**
```
Guitar → Compressor → PA-1QG → Overdrive → Delay → Reverb → Amp
```

**與其他器材搭配:**
- **Compressor:** Compressor 後接 PA-1QG，先控制動態再塑形音色
- **ODL-1-CS:** PA-1QG 後接 ODL-1-CS，EQ 塑形 + Dumble 音色
- **Buffer++:** Buffer++ 前接 PA-1QG，Always-on 設計

### 與其他 EQ 的差異

PA-1QG 最大優勢在於：
- **99 組可程式化預設** - 其他 EQ 通常只有 1-4 組
- **全類比訊號路徑** - 相較於數位 EQ 音色更溫暖
- **每預設獨立 LEVEL** - 可作為 Volume Controller
- **MIDI 支援完整** - 適合 MIDI 整合系統

---

**文件版本:** 1.0
**最後更新:** 2026-01-13
**下次更新計劃:** 補充實際使用者回饋與完整預設庫範例

**相關文件:**
- `shared/equipment_database/pedals/specs/pa1qg.yaml` - PA-1QG 完整技術規格
- `shared/equipment_database/pedals/specs/odl1cs.yaml` - ODL-1-CS 技術規格（同設計師）

---

**參考資料來源:**
- [Free the Tone 官方網站](https://www.freethetone.com/en/products/detail18/)
- [MusicRadar 評測（2018）](https://www.musicradar.com/reviews/free-the-tone-programmable-analog-eq)
- [Premier Guitar 報導（2018）](https://www.premierguitar.com/free-the-tone-unveils-programmable-analog-10-band-eq)
- [Pedal of the Day（2018）](https://www.pedal-of-the-day.com/2018/02/09/free-tone-pa-1qg-programmable-analog-10-band-eq/)
- Free the Tone 產品手冊
