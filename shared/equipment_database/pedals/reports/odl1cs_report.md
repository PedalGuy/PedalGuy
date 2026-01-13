# Free the Tone ODL-1-CS OVERDRIVELAND - 器材詳細報告

**版本:** 1.0
**更新日期:** 2026-01-13
**資料來源:** `shared/equipment_database/pedals/specs/odl1cs.yaml`

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
**型號:** ODL-1-CS (OVERDRIVELAND Custom Shop Version)
**類型:** Overdrive
**風格:** Dumble-style
**設計師:** Yuki Hayashi
**製造國:** Japan

### 核心賣點

Free the Tone ODL-1-CS 是一款捕捉傳奇 **Dumble Overdrive Special** 音箱質感的高階 Overdrive 效果器。設計師 Yuki Hayashi（Free the Tone 創辦人）擁有超過 20 年的 Dumble 音箱維修與調校經驗，並親自擁有多台 Dumble 音箱（包括 1992 年取得的 Dumble Overdrive Special 50W Combo），將這些經驗濃縮在這顆踏板中。

**獨特之處:**
- **雙通道設計** - Normal Channel（Clean 至輕度 Overdrive）+ Drive Channel（獨立破音模組）
- **Custom Shop 電壓可調** - 10-19V 連續可調，劇烈改變音色特性
- **無 Clipping Diodes** - Normal Channel 不使用二極體削波，保留豐富諧波
- **HTS Circuit** - Holistic Tonal Solution，最大化吉他音色特性的 Buffer 技術

### 適合的音樂風格

| 風格 | 適配度 | 說明 |
|------|--------|------|
| **Blues** | ⭐⭐⭐⭐⭐ | Dumble 經典應用，極佳動態反應 |
| **Jazz** | ⭐⭐⭐⭐⭐ | JAZZ 模式強調低頻，適合 Semi-Hollow |
| **Fusion** | ⭐⭐⭐⭐⭐ | Larry Carlton / Robben Ford 經典音色 |
| **Rock** | ⭐⭐⭐⭐ | ROCK 模式增加 Gain，適合 Rock 塑形 |
| **Neo Soul** | ⭐⭐⭐⭐ | 溫暖、豐富諧波，適合和弦演奏 |

**代表性藝術家:**
- Larry Carlton
- Robben Ford
- Eric Johnson
- Stevie Ray Vaughan
- John Mayer

---

## 技術規格詳解

### 電源規格

| 項目 | 規格 | 說明 |
|------|------|------|
| **外部供電** | DC 9V | Center Negative |
| **電流消耗** | 95mA | **需要 200mA 以上供電能力** |
| **內部升壓** | 10-19V 可調 (CS 版本) | Standard 版本固定 14.5V |
| **電池支援** | ❌ 不支援 | 高電流消耗，不適合電池供電 |

**⚠️ 重要提示:**
CS 版本的電壓調整功能是核心特色之一。透過內部 Trim 調整 10-19V 電壓，可以改變削波點（Clipping Point），劇烈改變破音質感：
- **10-12V** → 較早壓縮，溫暖、飽和
- **14-16V** → 標準設定，平衡動態與破音
- **17-19V** → 更大 Headroom，清晰、高動態

---

### 雙通道設計

#### **Normal Channel (主通道)**

**電路設計:**
- **無 Clipping Diodes/LEDs** - 不使用傳統二極體削波
- **豐富諧波** - 即使在 Clean 設定下也有輕微失真質感
- **Amp-like Response** - 如同音箱般有意識地回應

**控制旋鈕:**
1. **NOR LEVEL** - Normal Channel 輸出音量
2. **TONE** - 音色調整（可透過 GLASS 開關 Bypass）
3. **GAIN** - 增益控制

**切換開關:**

| 開關 | 功能 | 說明 |
|------|------|------|
| **EQ ON** | 啟動 Tone Circuit | 標準音色塑形 |
| **GLASS** | Bypass Tone Circuit | 類似 Blackface Fender Vibroverb 的 Bright Switch，玻璃般清晰 |
| **ROCK** | 增加 Gain + 削減低頻 | 避免 Amp 過載，適合 Rock 塑形 |
| **JAZZ** | 降低 Gain + 強調低頻 | 豐富低頻，適合 Jazz 音色 |

---

#### **Drive Channel (破音通道)**

**電路設計:**
- **獨立破音模組** - 不共用 Normal Channel 電路
- **位置在前** - Drive Channel 在 Normal Channel **之前**
- **Custom Module** - CS 版本使用不同零件，更敏感

**控制旋鈕:**
1. **DRV LEVEL** - Drive Channel 輸出音量
2. **DRIVE** - 破音強度
3. **PUSH** - 額外增益推動
4. **HI CUT** - 高頻削減（避免過亮）

**訊號流向:**
```
Guitar → Drive Channel → Normal Channel → Amp
```

---

### HTS Circuit (Holistic Tonal Solution)

**特性:**
- 不同於傳統 Buffer
- 最大化吉他音色特性
- 平衡音色與低噪音
- 輸出與輸入同相位
- **Buffered Bypass** (Always-on)

**阻抗規格:**
- **輸入阻抗:** 500kΩ or higher
- **輸出阻抗:** 10kΩ or higher

---

### Custom Shop vs Standard 版本差異

| 項目 | Standard 版本 | Custom Shop (CS) 版本 |
|------|--------------|---------------------|
| **Drive Module** | 標準模組 | 客製化模組（不同零件，更敏感） |
| **內部電壓** | 固定 14.5V | 10-19V 連續可調 |
| **音色特性** | 標準 Dumble 音色 | 更細膩、更敏感 |
| **價格** | $350-380 USD | $425 USD |

---

### 尺寸與重量

- **尺寸:** 97mm (D) × 120mm (W) × 51mm (H)
- **重量:** 約 420g（不含電池）

---

## 音色特性

### 核心音色特徵

1. **Dumble 特有的諧波豐富度**
   - 即使在 Clean 設定下，也帶有輕微失真質感
   - 諧波飽和但不泥濘

2. **Amp-like 反應**
   - 如同音箱有意識般回應撥弦力度
   - 極高的 Pick Sensitivity

3. **跨弦平衡**
   - 從 1 弦到 6 弦（或 7 弦）音量與音色平衡
   - 不會有特定弦過亮或過暗

4. **動態範圍極寬**
   - 輕撥 → Clean Tone with Sparkle
   - 重撥 → Saturated Overdrive
   - 吉他音量旋鈕極度敏感

---

### 頻率響應特性

**可透過開關大幅調整:**

| 模式 | 低頻 | 中頻 | 高頻 | 適合 |
|------|------|------|------|------|
| **JAZZ Mode** | 強調 | 平衡 | 溫暖 | Jazz, Blues, Neo Soul |
| **ROCK Mode** | 略減 | 突出 | 明亮 | Rock, Fusion, Drive Stacking |
| **GLASS Mode** | 平衡 | 平衡 | 極亮 | Clean Boost, Sparkle Tone |

---

### 壓縮特性

**Dumble-style Compression:**
- 自然的壓縮感（非機械式）
- 延音飽滿但不失 Attack
- 適合 Lead Solo 的持續音

---

## 使用範例

### 範例 1：Jazz Clean Tone (JAZZ Mode)

**音樂風格:** Jazz, Bossa Nova
**適合吉他:** Semi-Hollow（如 ESP Throbber-CTM）

**設定:**

| 通道 | 旋鈕 | 設定 |
|------|------|------|
| **Normal** | NOR LEVEL | 2 點鐘（Clean Boost） |
| **Normal** | TONE | 12 點鐘 |
| **Normal** | GAIN | 9 點鐘（Clean 設定） |
| **Drive** | 全關閉 | - |

**開關設定:**
- **EQ ON** ✅
- **JAZZ Mode** ✅
- **內部電壓:** 14V（標準）

**效果:**
- 溫暖、豐富的 Clean Tone
- 略帶壓縮感，延音自然
- 低頻豐富，適合和弦演奏
- Compressor 前置（如 Cali76 FET）可進一步強化

**訊號鏈位置:** Compressor → PA-1QG → **ODL-1-CS** → Amp

---

### 範例 2：Fusion Lead (Drive Channel + Normal Stacking)

**音樂風格:** Fusion, Blues
**適合吉他:** Humbucker 吉他（如 Greco TE-500）

**設定:**

| 通道 | 旋鈕 | 設定 |
|------|------|------|
| **Drive** | DRV LEVEL | 12 點鐘 |
| **Drive** | DRIVE | 11 點鐘（中等破音） |
| **Drive** | PUSH | 9 點鐘（輕推） |
| **Drive** | HI CUT | 10 點鐘（略削減高頻） |
| **Normal** | NOR LEVEL | 1 點鐘 |
| **Normal** | GAIN | 11 點鐘（輕度 Overdrive） |
| **Normal** | TONE | 1 點鐘 |

**開關設定:**
- **EQ ON** ✅
- **ROCK Mode** ✅
- **內部電壓:** 16V（增加動態）

**效果:**
- Drive Channel 提供基礎破音
- Normal Channel 再次推動，創造 Dumble 經典疊加
- 高動態反應，適合 Lead Solo
- Larry Carlton / Robben Ford 經典音色

**訊號鏈位置:** Compressor → **ODL-1-CS** → PA-1QG (Clean Boost) → Amp

---

### 範例 3：Rock Rhythm (ROCK Mode)

**音樂風格:** Rock, Blues Rock
**適合吉他:** 任何吉他

**設定:**

| 通道 | 旋鈕 | 設定 |
|------|------|------|
| **Normal** | NOR LEVEL | 12 點鐘 |
| **Normal** | TONE | 11 點鐘 |
| **Normal** | GAIN | 1 點鐘（中高 Gain） |
| **Drive** | 全關閉 | - |

**開關設定:**
- **EQ ON** ✅
- **ROCK Mode** ✅
- **內部電壓:** 12V（較早壓縮，溫暖）

**效果:**
- ROCK Mode 增加 Gain，略減低頻
- 避免音箱前級過載
- 適合 Power Chord 和 Riff
- 與其他 Overdrive 堆疊效果極佳

**Overdrive Stacking 建議:**
```
Sweet Honey (低 Gain) → ODL-1-CS (ROCK Mode) → Amp
```

---

### 範例 4：GLASS Mode (Clean Boost with Sparkle)

**音樂風格:** Neo Soul, Funk
**適合吉他:** Single-Coil 吉他（如 Fender Tokyo Thinline）

**設定:**

| 通道 | 旋鈕 | 設定 |
|------|------|------|
| **Normal** | NOR LEVEL | 3 點鐘（大音量提升） |
| **Normal** | TONE | - (Bypass 狀態) |
| **Normal** | GAIN | 8 點鐘（極低 Gain） |
| **Drive** | 全關閉 | - |

**開關設定:**
- **GLASS Mode** ✅ (Bypass Tone Circuit)
- **JAZZ Mode** ✅
- **內部電壓:** 17V（極大 Headroom）

**效果:**
- GLASS Mode 創造玻璃般清晰音色
- 類似 Blackface Fender 的 Bright Switch
- 適合 Single-Coil 增加高頻光澤
- Clean Boost 用途，不改變音色特性

**應用場景:**
- Solo 時提升音量與存在感
- 推動 Amp 進入輕度破音
- 搭配 Clean Amp（如 Roland JC-22）

---

### 範例 5：電壓實驗 (Custom Shop 專屬)

**實驗目的:** 找到個人喜好的音色特性

**實驗步驟:**

1. **基礎設定** (所有旋鈕 12 點鐘，JAZZ Mode, EQ ON)
2. **調整內部 Trim，測試不同電壓:**

| 電壓 | 音色特性 | 適合 |
|------|---------|------|
| **10V** | 早期壓縮，溫暖、飽和 | Blues, Vintage Tone |
| **12V** | 略早壓縮，溫暖 | Jazz, Neo Soul |
| **14V** | 標準設定，平衡 | 全能設定 |
| **16V** | 更大 Headroom，清晰 | Fusion, Clean Tone |
| **18V** | 極大 Headroom，高動態 | Hi-Fi, Studio Recording |
| **19V** | 最大 Headroom | 極端清晰，實驗性 |

3. **紀錄偏好電壓，作為日常設定**

**⚠️ 注意:**
- 電壓調整需打開效果器底蓋，使用小螺絲起子調整 Trim
- 調整後需重新測試所有設定

---

## 優缺點分析

### 優點 ✅

1. **成功捕捉 Dumble 音箱質感**
   - 20+ 年 Dumble 維修經驗濃縮在踏板中
   - 極高的音色還原度

2. **Custom Shop 電壓調整功能極有價值**
   - 10-19V 連續可調
   - 一顆效果器可涵蓋多種音色特性

3. **雙通道設計極度靈活**
   - 可單獨使用 Normal Channel（Clean Boost）
   - 可單獨使用 Drive Channel
   - 可兩者堆疊（Dumble 經典用法）

4. **HTS Circuit 提供優異訊號完整性**
   - 不同於傳統 Buffer
   - 最大化吉他音色特性

5. **開發嚴謹，品質可靠**
   - 開發耗時超過 3 年
   - 約 10 個原型測試
   - Free the Tone 日本製造品質

6. **極度敏感的動態反應**
   - Pick Attack 極度敏感
   - 吉他音量旋鈕反應極佳
   - 適合表現力強的演奏者

---

### 缺點 ❌

1. **價格高昂**
   - CS 版本 $425 USD
   - 屬於 High-End Boutique 等級

2. **不支援電池**
   - 95mA 高電流消耗
   - 需要 200mA 以上供電能力

3. **學習曲線較陡**
   - 雙通道設計複雜
   - 多種開關組合需要時間熟悉
   - CS 版本電壓調整需要實驗

4. **Buffered Bypass (Always-on)**
   - 無 True Bypass 選項
   - 對 True Bypass 純粹主義者可能是缺點

5. **體積較大**
   - 120mm 寬度
   - Pedalboard 空間佔用較多

---

### 適合人群 🎯

**最適合:**
- 追求 Dumble 音色但無法購買 Dumble 音箱的玩家
- Fusion, Jazz, Blues 玩家
- 對動態反應要求極高的演奏者
- Larry Carlton / Robben Ford 風格愛好者
- 願意花時間深入研究的玩家

**較不適合:**
- 預算有限的初學者
- 追求極端失真的 Metal 玩家
- 需要 True Bypass 的純粹主義者
- 希望即插即用、不想調整的玩家

---

## 網路驗證資訊

### 驗證來源

本報告的關鍵資訊已透過以下來源驗證：

1. **[Free the Tone 官方產品頁面](https://www.freethetone.com/en/products/detail73/)**
   - 完整技術規格
   - 官方設計理念說明

2. **[Premier Guitar 評測](https://www.premierguitar.com/free-the-tone-overdriveland)**
   - 專業評測與音色分析

3. **[Reverb 產品頁面](https://reverb.com/item/74730552-free-the-tone-custom-shop-overdriveland-odl-1-cs-authorized-dealer-free-shipping)**
   - 市場價格與用戶評價

### 驗證的關鍵資訊 ✓

- ✅ Yuki Hayashi 擁有 20+ 年 Dumble 維修經驗
- ✅ 開發耗時超過 3 年，約 10 個原型
- ✅ Normal Channel 無使用 Clipping Diodes/LEDs
- ✅ CS 版本可調 10-19V 電壓
- ✅ 建議售價 $425 USD (CS 版本)
- ✅ 電流消耗 95mA，需 200mA 以上供電
- ✅ Yuki Hayashi 親自擁有 Dumble Overdrive Special (1992) 和 Dumble Overdrive Reverb (1995)

### 設計背景補充

根據官方資訊，Yuki Hayashi 在開發 ODL-1-CS 時，選擇以「較晚期型號的 Dumble Overdrive Special」為藍本，因為這個版本具有「數位風格的特性」，更適合當代音樂，提供更強勁的 Rock 導向音色。

---

## 總結

### 核心優勢

Free the Tone ODL-1-CS 是市面上少數能真正捕捉 Dumble 音箱質感的踏板效果器之一。設計師 Yuki Hayashi 的 20+ 年 Dumble 維修經驗、嚴謹的開發過程（3 年，10 個原型），以及 Custom Shop 版本獨有的電壓調整功能，讓這顆效果器成為 Fusion, Jazz, Blues 玩家的終極選擇。

### 最佳使用建議

1. **初學者:** 從 JAZZ Mode 開始，Normal Channel 單獨使用，熟悉 Dumble 音色特性
2. **中階使用者:** 實驗 ROCK/GLASS 模式，嘗試雙通道堆疊
3. **進階使用者 (CS 版本):** 調整內部電壓，找到個人偏好的音色特性，建立完整的 Overdrive Stacking 系統

### 訊號鏈定位

**最佳位置:** Signal Chain 前段 (Pre-Amp Gain Section)

**推薦配置:**
```
Guitar → Compressor → EQ → ODL-1-CS → (其他 Overdrive) → Delay → Reverb → Amp
```

**Overdrive Stacking 範例:**
```
Sweet Honey (Warm Base) → ODL-1-CS (ROCK Mode, Dumble Push) → Amp
```

---

**文件版本:** 1.0
**最後更新:** 2026-01-13
**下次更新計劃:** 補充實際使用者回饋與 Overdrive Stacking 進階範例

**相關文件:**
- `shared/equipment_database/pedals/specs/odl1cs.yaml` - ODL-1-CS 完整技術規格
- `projects/2025-v3-signal-chain/research/overdrive_pedals_technical_data.md` - Overdrive 技術資料

---

**參考資料來源:**
- [Free the Tone 官方網站](https://www.freethetone.com/en/products/detail73/)
- [Premier Guitar 評測](https://www.premierguitar.com/free-the-tone-overdriveland)
- Free the Tone 產品手冊
- Yuki Hayashi 設計資料
