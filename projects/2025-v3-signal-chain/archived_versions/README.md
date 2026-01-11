# 歸檔版本說明

**最後歸檔日期:** 2026-01-10
**歸檔原因:** 專案演進，從雙音箱配置（JC-22 + Tone King）轉換為單 Tone King Preamp 配置，同時從 Swiss Things 升級到 Empress Buffer++

---

## 歸檔文件列表

### Signal Chains 目錄歸檔

#### signal_chain_v3.0_dual_amp_archived.md
- **原始版本:** V3.0
- **創建日期:** 2025-12-30
- **說明:** 基於雙音箱配置（Roland JC-22 + Tone King Imperial）的訊號鏈設計
- **被取代原因:** 2026-01-08 改為單 Tone King Preamp 配置
- **對應的最終版本:** signal_chains/signal_chain_toneking_only.md

#### signal_chain_diagrams_v3.0_dual_amp_archived.md
- **原始檔名:** signal_chain_diagrams_v2.md
- **原始版本:** V3.0（檔名雖為 v2 但內容為 V3.0）
- **創建日期:** 2025-12-30
- **說明:** V3.0 雙音箱配置的 Mermaid 流程圖
- **被取代原因:** 2026-01-08 改為單 Tone King Preamp 配置
- **對應的最終版本:** signal_chains/signal_chain_toneking_only.md

#### signal_chain_diagrams_v2.0_archived.md
- **原始版本:** V2.0
- **創建日期:** 2025-12-30
- **說明:** 基於 V2.0 效果器配置（使用 Colosseum）的訊號鏈流程圖
- **被取代原因:** V3.0 版本移除了 Colosseum，改用 PRS Horsemeat + JHS Morning Glory V3

---

### Analysis 目錄歸檔

#### comprehensive_analysis_summary_v2.0_dual_amp_archived.md
- **原始版本:** V2.0
- **完成日期:** 2025-12-30
- **說明:** 基於雙音箱配置的完整分析報告（10顆核心效果器）
- **被取代原因:** 2026-01-08 改為單 Tone King Preamp 配置
- **對應的最終版本:** signal_chains/signal_chain_toneking_only.md

#### signal_chain_master_plan_v1.0_archived.md
- **原始版本:** V1.0
- **建立日期:** 2025-12-13
- **說明:** 初始版本的訊號鏈總計畫（17顆效果器）
- **被取代原因:** V2.0 版本優化為 10 顆核心效果器
- **對應的最終版本:** 已被後續版本取代

#### swiss_things_integration_plan_v2.0_dual_amp_archived.md
- **原始版本:** V2.0
- **建立日期:** 2025-12-30
- **說明:** V3.0 效果器配置的 Swiss Things 整合方案
- **被取代原因:** 2026-01-02 發現 Buffer++ 更適合（支援 Stereo FX Loop），並於 2026-01-08 確定使用 Buffer++
- **對應的最終版本:** 已由 Empress Buffer++ 配置取代

#### swiss_things_integration_plan_v1.0_archived.md
- **原始版本:** V1.0
- **創建日期:** 2025-12-30
- **說明:** 基於 V2.0 效果器配置（使用 Colosseum）的 Swiss Things 整合方案
- **被取代原因:** V3.0 版本效果器配置變更（移除 Colosseum）

#### comprehensive_analysis_summary_v1.0_archived.md
- **原始版本:** V1.0
- **創建日期:** 2025-12-13
- **說明:** 初始版本的完整分析報告（17顆效果器）
- **被取代原因:** V2.0 版本優化為 10 顆核心效果器

---

### Research 目錄歸檔

#### swiss_things_signal_routing_logic_archived.md
- **原始版本:** 1.0
- **建立日期:** 2025-12-22
- **說明:** Swiss Things 訊號路徑邏輯完整文件
- **被取代原因:** 2026-01-02 決定升級至 Empress Buffer++（支援 Stereo Loop 2）
- **參考價值:** 了解 Swiss Things 的路由邏輯，以及為何選擇 Buffer++
- **相關文件:** analysis/buffer_plus_plus_vs_swiss_things_comparison.md（決策依據）

---

## 版本演進歷史

### V1.0 → V2.0（效果器配置優化）
**日期:** 2025-12-13 → 2025-12-30

**主要變更:**
- 效果器數量：17 顆 → 12 顆 → **10 顆**
- 移除 From Yesterday (KOT Clone) - 功能被 PA-1QG LEVEL 取代
- 移除 Soul Food - 功能被 Colosseum Klon Side 取代
- 移除 JHS Morning Glory V3 - 功能與 Colosseum BB Side 重疊
- 移除 Virtues Arca - 功能與 Colosseum BB Side 重疊
- 提升 TWA Source Code 至核心效果器

### V2.0 → V3.0（訊號鏈配置優化）
**日期:** 2025-12-30

**主要變更:**
- **移除:** Cornerstone Colosseum（雙通道 OD）
- **新增:** PRS Horsemeat（訊號鏈1 的 Klon-style Boost）
- **新增:** JHS Morning Glory V3（訊號鏈2 的 Bluesbreaker OD）
- **理念:** 單功能專用效果器，訊號鏈更單純易懂
- **效果器總數:** 10 顆 → 11 顆核心效果器
- **配置:** 雙音箱（Roland JC-22 + Tone King Imperial）
- **路由器:** EarthQuaker Swiss Things

### V3.0 → Toneking Only（單音箱配置）
**日期:** 2026-01-08

**主要變更:**
- **移除音箱:** Roland JC-22
- **保留:** Tone King Imperial MKII Preamp Pedal
- **路由器升級:** Swiss Things → **Empress Buffer++**
  - 升級原因：Buffer++ Loop 2 支援 Stereo（Swiss Things 僅 Mono）
  - 充分發揮 Tone King Stereo FX Loop + Stereo XLR 輸出
- **新增:** Boss CE-2W Waza Craft Chorus
  - 補償 JC-22 的 Dimensional Space Chorus
  - CE-1 模式 = JC-120 Chorus 來源
- **空間系順序優化:** AASB (Mono) → Nucleo (Stereo) → FF-1Y (保留 Stereo)
- **效果器總數:** 12 顆（11 顆核心 + Buffer++ + CE-2W）

**關鍵決策文件:**
- `analysis/buffer_plus_plus_vs_swiss_things_comparison.md` (2026-01-02)
  - 發現 JC-22 和 Tone King 都支援 Stereo FX Loop
  - Buffer++ Loop 2 Stereo 可充分發揮音箱的 Stereo 能力
  - Swiss Things Loop 2 Mono 無法利用 Stereo FX Loop

---

## 型號更正記錄

### FF-1Y vs FT-1Y 更正（2026-01-10）
**發現問題:** 效果器型號記錄錯誤

**錯誤型號:** Free the Tone FT-1Y Flight Time Digital Delay
**正確型號:** Free the Tone FF-1Y FUTURE FACTORY

**主要差異:**
- FF-1Y 具備雙延遲模組（FT-1Y 為單模組）
- FF-1Y 支援立體聲（FT-1Y 為單聲道）
- FF-1Y 有 3-band EQ（FT-1Y 為 LPF/HPF）
- FF-1Y 有 Soft Clipping circuit
- FF-1Y 為 Random Fluctuating Phase Modulation（FT-1Y 為標準調變）
- FF-1Y 使用 9V 電源（FT-1Y 為 12V）

**更正檔案:** 已建立 `shared/equipment_database/pedals/ff1y.yaml`
**舊檔歸檔:** `shared/equipment_database/pedals/archived/ft1y_incorrect.yaml`

---

## 如何使用歸檔文件

這些歸檔文件保留了專案的演進歷史，可用於：

1. **參考歷史決策過程** - 了解為什麼從雙音箱改為單 Preamp，為什麼從 Swiss Things 升級到 Buffer++
2. **對比不同配置方案** - 比較 V1.0、V2.0、V3.0、Toneking Only 的差異
3. **恢復舊配置** - 如果需要回到雙音箱配置
4. **學習優化思路** - 理解從 17 顆效果器優化到 12 顆核心配置的過程

---

## 最終版本文件位置

**最終版本的文件請參考:**

### Signal Chains 目錄
- ✅ `signal_chains/signal_chain_toneking_only.md` - **Toneking Only v1.0 最終配置（2026-01-08）**

### Analysis 目錄
- ⚠️ 已全部歸檔（基於雙音箱或 Swiss Things 配置，已不適用）
- 📄 參考決策文件：`/analysis/buffer_plus_plus_vs_swiss_things_comparison.md`（位於專案根目錄）

### Research 目錄
- ✅ `research/compressor_eq_spatial_effects_technical_data.md` - 壓縮器/EQ/空間系技術資料（已更正 FF-1Y）
- ✅ `research/guitar_amp_pairing_guide.md` - 吉他音箱配對指南
- ✅ `research/guitar_collection_analysis.md` - 吉他收藏分析
- ✅ `research/overdrive_pedals_technical_data.md` - 破音效果器技術資料
- ✅ `research/overdrive_stacking_analysis.md` - 破音效果器疊加分析

---

**歸檔負責人:** Claude Code (Sonnet 4.5)
**最後更新:** 2026-01-10
