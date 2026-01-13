# TWA Source Code Overdrive - 器材詳細報告

**版本:** 1.0
**更新日期:** 2026-01-13
**資料來源:** `shared/equipment_database/pedals/specs/twa_source_code.yaml`

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

**品牌:** TWA (Totally Wycked Audio)
**型號:** Source Code Overdrive
**全名:** TWA Source Code - Next-Gen Tube Screamer Evolution
**設計師:** Susumu Tamura (原始 TS808 創造者)
**類型:** Overdrive
**風格:** Tube Screamer Evolution (TS808 終極進化版)
**製造國:** USA
**製造方式:** 美國手工製作
**價格:** $299 USD

### 核心賣點

TWA Source Code 是由 **Susumu Tamura** (1979 年創造 Ibanez TS808 Tube Screamer 的傳奇設計師) 親自設計的 **Tube Screamer 終極進化版本**。這款效果器不是單純的 TS808 複刻或修改版，而是 Tamura 先生基於 40 多年的電路設計經驗，對 Tube Screamer 架構進行全面革新的作品。

Source Code 的核心創新在於全新的 **BITE Control** (咬合控制)，這是一個前所未有的旋鈕，可以調整**偶次諧波與奇次諧波的平衡**，讓玩家從對稱削波 (Symmetrical Clipping) 無縫過渡到不對稱削波 (Asymmetrical Clipping)，創造從平滑 Overdrive 到高增益真空管音箱感的極端音色範圍。

搭配 **18V 內部電壓** (透過內部穩壓器從 9V 升壓)、**全新 Multi-Transistor Input Buffer**、**Magic IC OpAmp** 以及 **+6dB Boost Circuit**，Source Code 成為市面上最接近「完美 TS808-style Overdrive」的效果器。

**獨特之處:**
- **BITE Control** - 世界首創偶次/奇次諧波平衡調整
- **18V 內部電壓** - 從 9V 升壓至 18V，增加 Headroom 與動態
- **原始 TS808 創造者設計** - Susumu Tamura 親自操刀
- **Multi-Transistor Input Buffer** - 全新 Buffer 設計，保護音色完整性
- **Magic IC OpAmp** - 增加諧波內容與類比感
- **+6dB Boost Circuit** - 可當 Clean Boost 使用
- **True Bypass** - 保持訊號純淨

### 適合的音樂風格

| 風格 | 適配度 | 說明 |
|------|--------|------|
| **Blues** | ⭐⭐⭐⭐⭐ | TS 經典應用，BITE Control 提供極佳表現力 |
| **Rock** | ⭐⭐⭐⭐⭐ | 中頻突出，適合 Rhythm 與 Lead |
| **Fusion** | ⭐⭐⭐⭐⭐ | 動態反應極佳，適合 Larry Carlton 風格 |
| **Classic Rock** | ⭐⭐⭐⭐⭐ | TS-style 中頻 Boost 經典音色 |
| **Modern Styles** | ⭐⭐⭐⭐⭐ | 18V 高 Headroom 適合現代音色 |
| **Country** | ⭐⭐⭐⭐ | Clean Boost 與輕度 Overdrive |
| **Metal** | ⭐⭐⭐ | 適合 Boost 其他 Overdrive，但非主力 |

**代表性藝術家 (TS808 使用者):**
- Stevie Ray Vaughan
- Gary Moore
- John Mayer
- Eric Johnson
- Noel Gallagher (Oasis)

---

## 技術規格詳解

### 電源規格

| 項目 | 規格 | 說明 |
|------|------|------|
| **外部供電** | DC 9V | Center Negative |
| **內部電壓** | **18V** | 透過內部穩壓器升壓 |
| **電流消耗** | 待確認 (估計 50-80mA) | 標準 Overdrive 範圍 |
| **電池支援** | ❌ 不支援 (推測) | 需要穩定外部供電 |

**⚠️ 重要提示:**
- Source Code 透過內部穩壓器將 9V 升壓至 **18V 運作**
- 18V 電壓提供更大 Headroom、更好的動態範圍與更清晰的音色
- 這是相較於標準 TS808 (9V) 的重大升級

---

### 控制旋鈕詳解

#### **主要旋鈕**

1. **LEVEL (輸出音量)**
   - **功能:** 控制效果器輸出音量
   - **範圍:** Unity Gain ~ +6dB Boost
   - **應用:** 可當 Clean Boost 使用 (低 Drive 設定 + 高 Level)

2. **DRIVE (增益控制)**
   - **功能:** 控制破音/增益量
   - **範圍:** Clean Boost ~ High Gain Overdrive
   - **特性:** 比標準 TS808 增益範圍更廣

3. **TONE (音色控制)**
   - **功能:** 調整音色明暗
   - **範圍:** 溫暖 ~ 明亮
   - **特性:** TS-style 音色控制，著重於中高頻調整

4. **BITE (咬合控制) ⭐ 核心創新**
   - **功能:** 調整偶次/奇次諧波平衡
   - **範圍:**
     - **最小值 (逆時針):** 對稱削波 (Symmetrical Clipping) → 偶次諧波為主 → 平滑、溫暖
     - **中間值 (12 點鐘):** 平衡設定
     - **最大值 (順時針):** 不對稱削波 (Asymmetrical Clipping) → 奇次諧波為主 → 高增益真空管音箱感
   - **音色影響:**
     - 低 BITE → 平滑、柔和、類似 Clean Boost
     - 中 BITE → 標準 TS808 音色
     - 高 BITE → 高增益真空管音箱感、更多壓縮、更飽和

---

### BITE Control 詳解 (核心創新)

#### **什麼是偶次/奇次諧波?**

**偶次諧波 (Even-Order Harmonics):**
- 音樂性較強
- 聽起來平滑、溫暖、飽滿
- 類似真空管放大器或 Tape 飽和
- 與原始音符和諧共鳴

**奇次諧波 (Odd-Order Harmonics):**
- 攻擊性較強
- 聽起來明亮、有力、銳利
- 類似晶體管放大器或固態放大器
- 增加「咬合感」(Bite)

---

#### **BITE Control 如何運作?**

**對稱削波 (Symmetrical Clipping):**
- 正負波形被相同方式削波
- 產生偶次諧波為主
- 音色平滑、溫暖

**不對稱削波 (Asymmetrical Clipping):**
- 正負波形被不同方式削波
- 產生奇次諧波為主
- 音色攻擊性強、有力

**BITE Control 讓玩家在兩者之間無縫調整:**
```
低 BITE (對稱削波) ←→ 中 BITE (平衡) ←→ 高 BITE (不對稱削波)
平滑、溫暖           標準 TS808     高增益真空管感
```

---

#### **BITE Control 建議起始點**

**Susumu Tamura 建議:**
- 從 **12 點鐘** 開始調整
- 根據個人喜好往左 (平滑) 或往右 (攻擊) 微調

**快速設定指南:**

| 音色需求 | BITE 設定 | 說明 |
|---------|----------|------|
| **Clean Boost** | 9 點鐘 (低) | 平滑、透明、不改變音色 |
| **Blues Crunch** | 11 點鐘 | 溫暖、飽滿、類比感 |
| **標準 TS808** | 12 點鐘 | 平衡設定 |
| **Rock Lead** | 1 點鐘 | 略增加攻擊性 |
| **High Gain** | 2-3 點鐘 (高) | 高增益真空管音箱感 |

---

### 18V Operation 優勢

#### **為什麼升壓至 18V?**

**標準 TS808 (9V 運作) 限制:**
- Headroom 較小
- 動態範圍受限
- 高輸出吉他容易過載

**Source Code (18V 運作) 優勢:**

1. **更大 Headroom**
   - 不易削波過度
   - 保留更多原始音色

2. **更好的動態範圍**
   - 輕撥 → 清晰
   - 重撥 → 飽和
   - 極度敏感的 Pick Attack

3. **更清晰的音色**
   - 高頻更開放
   - 低頻更飽滿
   - 較少泥濘感

4. **更好的音色分離**
   - 和弦演奏時每個音符更清晰
   - 適合複雜和弦

---

### Multi-Transistor Input Buffer

**傳統 TS808 Buffer:**
- 單一電晶體 Buffer
- 阻抗匹配基本

**Source Code Multi-Transistor Buffer:**
- 全新多電晶體設計
- 最大化保護吉他音色特性
- 平衡音色與低噪音
- **Always-on Buffer** (不可 Bypass)

**優勢:**
- 保護吉他拾音器訊號
- 驅動長導線或多顆效果器
- 保持高頻清晰度

---

### Magic IC OpAmp

**功能:**
- 增加諧波內容
- 創造更具類比感的音色
- 更接近真空管音箱的反應

**Tamura 設計理念:**
- 不透露具體 IC 型號 (保持神秘感)
- 稱之為「Magic IC」強調其特殊性

---

### +6dB Boost Circuit

**功能:**
- LEVEL 旋鈕可提供最高 +6dB 增益
- 不改變音色特性

**應用:**
- Clean Boost (低 Drive + 高 Level)
- Solo 時提升音量
- 推動音箱前級

---

### Bypass 技術

**規格:**
- **True Bypass**
- 不使用 Buffered Bypass
- 效果關閉時訊號完全不經過電路

**注意:**
- Input Buffer 是 **Always-on** (即使效果關閉也運作)
- 這是 TS-style Overdrive 的標準設計

---

## 音色特性

### 核心音色特徵

1. **TS808 基因，但更進化**
   - 保留經典 TS 中頻特色
   - 透過 18V 與 BITE Control 提供更多彈性

2. **極度敏感的動態反應**
   - 18V 電壓提供寬廣動態範圍
   - Pick Attack 極度敏感
   - 吉他音量旋鈕反應極佳

3. **BITE Control 創造極端音色範圍**
   - 從平滑 Clean Boost 到高增益真空管感
   - 一顆踏板涵蓋多種音色特性

4. **比標準 TS808 更透明**
   - 18V Headroom 減少泥濘感
   - 高頻更開放
   - 低頻更飽滿

5. **Amp-like 反應**
   - Magic IC OpAmp 創造類比感
   - 如同音箱般回應撥弦力度

---

### 頻率響應特性

**與標準 TS808 比較:**

| 頻段 | TS808 | Source Code | 說明 |
|------|-------|------------|------|
| **低頻** | 略減 | **更飽滿** | 18V 提供更好低頻表現 |
| **中頻** | 突出 | **保留但更平衡** | TS 特色中頻，但較不堆疊 |
| **高頻** | 略暗 | **更開放** | 18V 高頻更清晰，較不刺耳 |

---

### 增益範圍比較

| 設定 | TS808 | Source Code | 說明 |
|------|-------|------------|------|
| **Clean Boost** | 略難達成 | **極佳** | 低 BITE + 低 Drive |
| **輕度 Overdrive** | ✅ | ✅ | 經典 TS 音色 |
| **中度 Overdrive** | ✅ | ✅ | 標準設定 |
| **高增益 Overdrive** | ❌ 較難達成 | **✅ 可達成** | 高 BITE + 高 Drive |

**結論:** Source Code 增益範圍比 TS808 更廣

---

### 壓縮特性

**可透過 BITE 調整:**

| BITE 設定 | 壓縮感 | 說明 |
|----------|--------|------|
| **低 (對稱削波)** | 適中 | 自然壓縮，延音飽滿 |
| **中 (平衡)** | 適中至略高 | 標準 TS808 壓縮感 |
| **高 (不對稱削波)** | 高 | 明顯壓縮，高增益真空管感 |

---

## 使用範例

### 範例 1：Clean Boost (低 BITE)

**音樂風格:** Jazz, Country, Clean Tones
**適合吉他:** 任何吉他

**設定:**

| 參數 | 設定 |
|------|------|
| **LEVEL** | 2-3 點鐘 (高音量) |
| **DRIVE** | 8-9 點鐘 (極低) |
| **TONE** | 12 點鐘 (中性) |
| **BITE** | 9 點鐘 (低，對稱削波) |

**效果:**
- 平滑、透明的 Clean Boost
- 不改變音色特性
- 提升音量與存在感
- 推動音箱前級

**訊號鏈位置:**
```
Guitar → Source Code (Clean Boost) → Amp
```

---

### 範例 2：Blues Crunch (中低 BITE)

**音樂風格:** Blues, Blues Rock
**適合吉他:** Single-Coil 吉他 (Stratocaster)

**設定:**

| 參數 | 設定 |
|------|------|
| **LEVEL** | 12 點鐘 (Unity Gain) |
| **DRIVE** | 11 點鐘 (中低增益) |
| **TONE** | 1 點鐘 (略明亮) |
| **BITE** | 11 點鐘 (中低，略偶次諧波) |

**效果:**
- 溫暖、飽滿的 Blues Crunch
- 偶次諧波創造類比感
- 極度敏感的 Pick Attack
- Stevie Ray Vaughan 風格

**訊號鏈位置:**
```
Guitar → Compressor (輕度) → Source Code (Blues Crunch) → Amp
```

---

### 範例 3：標準 TS808 音色 (中 BITE)

**音樂風格:** Rock, Classic Rock
**適合吉他:** 任何吉他

**設定:**

| 參數 | 設定 |
|------|------|
| **LEVEL** | 12 點鐘 (Unity Gain) |
| **DRIVE** | 12 點鐘 (中等增益) |
| **TONE** | 12 點鐘 (中性) |
| **BITE** | **12 點鐘** (平衡，標準 TS808) |

**效果:**
- 經典 TS808 中頻突出音色
- 但比 TS808 更清晰 (18V 優勢)
- 適合 Rhythm 與 Lead
- 與其他 Overdrive 堆疊效果極佳

**Overdrive Stacking 範例:**
```
Guitar → Bluesbreaker (低 Gain) → Source Code (標準 TS808) → Amp
```

---

### 範例 4：Rock Lead Solo (中高 BITE)

**音樂風格:** Rock, Fusion
**適合吉他:** Humbucker 吉他

**設定:**

| 參數 | 設定 |
|------|------|
| **LEVEL** | 1 點鐘 (略 Boost) |
| **DRIVE** | 1 點鐘 (中高增益) |
| **TONE** | 1 點鐘 (明亮) |
| **BITE** | 1 點鐘 (中高，略增加奇次諧波) |

**效果:**
- 略增加攻擊性的 Lead 音色
- 中頻突出，在 Mix 中容易辨識
- 高動態反應，適合表現力演奏
- Larry Carlton / Robben Ford 風格

**訊號鏈位置:**
```
Guitar → Source Code (Rock Lead) → Delay → Reverb → Amp
```

---

### 範例 5：High Gain Tube Amp Simulation (高 BITE)

**音樂風格:** High Gain Rock, Modern Rock
**適合吉他:** Humbucker 吉他

**設定:**

| 參數 | 設定 |
|------|------|
| **LEVEL** | 11 點鐘 (略減音量) |
| **DRIVE** | 2-3 點鐘 (高增益) |
| **TONE** | 11 點鐘 (略削減高頻避免刺耳) |
| **BITE** | **2-3 點鐘** (高，不對稱削波，奇次諧波) |

**效果:**
- 高增益真空管音箱感
- 明顯壓縮與飽和
- 奇次諧波創造攻擊性
- 適合 Power Chord 與 Riff

**訊號鏈位置:**
```
Guitar → Source Code (High Gain) → Amp (Clean Channel)
```

或

```
Guitar → Source Code (High Gain) → Amp (Crunch Channel) → 極端飽和
```

---

### 範例 6：Overdrive Stacking - TS Boost

**音樂風格:** High Gain Rock, Metal (非主力，但可用)
**適合吉他:** 任何吉他

**設定:**

| 參數 | 設定 |
|------|------|
| **LEVEL** | 2 點鐘 (Boost) |
| **DRIVE** | 10 點鐘 (低增益) |
| **TONE** | 11 點鐘 (略削減高頻) |
| **BITE** | 12 點鐘 (標準) |

**訊號鏈:**
```
Guitar → High Gain Distortion (如 Friedman BE-OD) → Source Code (TS Boost) → Amp
```

**效果:**
- Source Code 作為 TS Boost 推動前方 Distortion
- 中頻突出，增加 Clarity
- 略削減低頻避免過於混濁
- 經典 TS Boost 用法

---

## 優缺點分析

### 優點

1. **原始 TS808 創造者設計**
   - Susumu Tamura 親自操刀
   - 具有權威性與歷史意義

2. **BITE Control 是遊戲規則改變者**
   - 前所未有的偶次/奇次諧波控制
   - 一顆踏板涵蓋極端音色範圍

3. **18V Operation 提供顯著優勢**
   - 更大 Headroom
   - 更好的動態範圍
   - 更清晰的音色

4. **比標準 TS808 更透明**
   - 較少中頻堆疊
   - 高頻更開放
   - 低頻更飽滿

5. **極度敏感的動態反應**
   - Pick Attack 極度敏感
   - 吉他音量旋鈕反應極佳

6. **Multi-Transistor Input Buffer**
   - 全新 Buffer 設計
   - 保護音色完整性

7. **+6dB Boost Circuit**
   - 可當 Clean Boost 使用
   - 不改變音色特性

8. **美國手工製作**
   - TWA 品質可靠
   - $299 價格合理 (相較於其他 Boutique TS)

9. **與其他 Overdrive 堆疊效果極佳**
   - TS-style 中頻特性適合堆疊

---

### 缺點

1. **價格較高**
   - $299 USD
   - 比標準 TS808 貴約 $100

2. **學習曲線 (BITE Control)**
   - 需要時間理解偶次/奇次諧波概念
   - 建議從 12 點鐘開始實驗

3. **Always-on Buffer**
   - Input Buffer 無法 Bypass
   - True Bypass 純粹主義者可能介意

4. **不支援電池 (推測)**
   - 需要穩定外部供電

5. **TS-style 中頻特性保留**
   - 雖然比 TS808 更平衡，但仍有 TS 中頻特色
   - 不適合追求完全透明 Overdrive 的玩家

6. **品牌知名度較低**
   - TWA 相較於 Ibanez/Boss 知名度較低
   - 部分玩家可能不熟悉

---

### 適合人群

**最適合:**
- TS808 愛好者 (追求進化版)
- Blues, Rock, Fusion 玩家
- 追求高動態反應的演奏者
- 需要 Clean Boost 與 Overdrive 兩用的玩家
- Overdrive Stacking 愛好者
- 追求 Boutique TS-style Overdrive 的玩家
- Susumu Tamura 粉絲 (歷史意義)

**較不適合:**
- 預算有限的初學者 (考慮標準 TS808 或 TS9)
- 追求完全透明 Overdrive 的玩家 (考慮 Bluesbreaker-style)
- 追求極端失真的 Metal 玩家 (TS 非 Metal 主力)
- True Bypass 純粹主義者 (Always-on Buffer)
- 不喜歡 TS 中頻特性的玩家

---

## 網路驗證資訊

### 驗證來源

本報告的關鍵資訊已透過以下來源驗證:

1. **[TWA 官方產品頁面](https://totallywyckedaudio.com/products/sc-01-source-code-overdrive)**
   - 完整技術規格
   - 官方產品描述

2. **[Guitar World 評測](https://www.guitarworld.com/gear/effects-pedals/twa-source-code-review)**
   - 「接近完美的 TS808-style 踏板，由 Tube Screamer 創造者設計，可以說是新的黃金標準」
   - 專業評測與音色分析

3. **[Guitar World 新聞](https://www.guitarworld.com/gear/guitar-pedals/twa-source-code)**
   - Tube Screamer 是最具代表性的 Overdrive 之一，現在由最初開發它的踏板先驅重新發明

4. **[Premier Guitar 報導](https://www.premierguitar.com/news/twa-introduces-source-code-overdrive)**
   - TWA 推出 Source Code Overdrive

5. **[Guitar Pedal X 報導](https://www.guitarpedalx.com/news/gpx-blog/susumu-tamura-the-original-creator-of-the-tube-screamer-pedal-makes-the-next-evolution-of-that-format-for-totally-wycked-audio-as-the-new-source-code-overdrive-with-unique-bite-control-and-refinements-in-every-area)**
   - Susumu Tamura - Tube Screamer 原始創造者 - 為 TWA 打造該格式的下一個進化版本

6. **[Godlyke 經銷商頁面](https://godlyke.com/products/sc-01-source-code-overdrive)**
   - 規格確認與經銷資訊

### 驗證的關鍵資訊

- ✅ 設計師 Susumu Tamura (1979 年創造 TS808)
- ✅ BITE Control 調整偶次/奇次諧波平衡
- ✅ 18V 內部電壓 (從 9V 升壓)
- ✅ Multi-Transistor Input Buffer
- ✅ Magic IC OpAmp
- ✅ +6dB Boost Circuit
- ✅ True Bypass
- ✅ 美國手工製作
- ✅ 建議售價 $299 USD
- ✅ 控制旋鈕: Level / Drive / Tone / Bite

### Guitar World 評測摘要

> "A near-perfect TS808-style pedal from the designer of the Tube Screamer that could arguably be the new gold standard."
> (接近完美的 TS808-style 踏板，由 Tube Screamer 設計師打造，可以說是新的黃金標準。)

> "It's hard to beat a classic, but the TWA Source Code overdrive, a leveled-up TS808-style pedal refined by the creator of the original Tube Screamer, has done just that."
> (很難擊敗經典，但 TWA Source Code overdrive，這款由原始 Tube Screamer 創造者改良的進化 TS808-style 踏板，做到了。)

### 用戶評價摘要 (TWA 官網)

**正面評價:**
- 「立即成為我最喜歡的 Overdrive」
- 「沒有中頻 honk。這可能是最好的 Tube Screamer」
- 「BITE Control 是遊戲規則改變者」
- 「18V 帶來的 Headroom 差異明顯」

---

## 總結

### 核心優勢

TWA Source Code 是 Susumu Tamura (原始 TS808 創造者) 基於 40 多年經驗打造的 **Tube Screamer 終極進化版本**。全新的 **BITE Control** 提供前所未有的偶次/奇次諧波調整能力，讓玩家從平滑 Clean Boost 無縫過渡到高增益真空管音箱感。

**18V 內部電壓** 提供更大 Headroom 與更好的動態範圍，**Multi-Transistor Input Buffer** 保護音色完整性，**Magic IC OpAmp** 增加諧波內容，**+6dB Boost Circuit** 提供 Clean Boost 功能。這些技術革新讓 Source Code 成為「可能是新的 TS808 黃金標準」。

### 最佳使用建議

1. **初學者:** BITE 從 12 點鐘開始，Drive 11 點鐘，體驗標準 TS808 音色
2. **中階使用者:** 實驗不同 BITE 設定，找到個人偏好的諧波平衡
3. **進階使用者:** 利用 BITE Control 創造極端音色，建立完整的 Overdrive Stacking 系統

### BITE Control 快速指南

```
9 點鐘 ←→ 11 點鐘 ←→ 12 點鐘 ←→ 1 點鐘 ←→ 2-3 點鐘
Clean    Blues      標準      Rock     High Gain
Boost    Crunch     TS808     Lead     Tube Amp
對稱削波            平衡              不對稱削波
偶次諧波                              奇次諧波
```

### 訊號鏈定位

**最佳位置:** Signal Chain 前段或中段 (Pre-Amp Gain Section)

**推薦配置:**
```
Guitar → Compressor → Source Code → Amp
```

**Overdrive Stacking 範例:**
```
Guitar → Bluesbreaker (低 Gain) → Source Code (TS Boost) → Amp
```

**Clean Boost 用途:**
```
Guitar → Source Code (Clean Boost, 低 BITE) → Amp → Solo 音量提升
```

---

**文件版本:** 1.0
**最後更新:** 2026-01-13
**下次更新計劃:** 補充實際使用者回饋與 BITE Control 進階應用範例

**相關文件:**
- `shared/equipment_database/pedals/specs/twa_source_code.yaml` - Source Code 完整技術規格
- `projects/2025-v3-signal-chain/research/overdrive_pedals_technical_data.md` - Overdrive 技術資料

---

**參考資料來源:**
- [TWA 官方產品頁面](https://totallywyckedaudio.com/products/sc-01-source-code-overdrive)
- [Guitar World 評測](https://www.guitarworld.com/gear/effects-pedals/twa-source-code-review)
- [Guitar World 新聞](https://www.guitarworld.com/gear/guitar-pedals/twa-source-code)
- [Premier Guitar 報導](https://www.premierguitar.com/news/twa-introduces-source-code-overdrive)
- [Guitar Pedal X 報導](https://www.guitarpedalx.com/news/gpx-blog/susumu-tamura-the-original-creator-of-the-tube-screamer-pedal-makes-the-next-evolution-of-that-format-for-totally-wycked-audio-as-the-new-source-code-overdrive-with-unique-bite-control-and-refinements-in-every-area)
- [Godlyke 經銷商頁面](https://godlyke.com/products/sc-01-source-code-overdrive)
