# 使用範例文件生成機制 - 分析與建議

**分析日期:** 2026-01-11
**分析對象:** 根據 YAML/Research 建立效果器使用範例文件的完整工作流程

---

## 問題 1: 是否建立一個以 YAML 或 Research 結果建立範例文件的 Skill?

### 回答：✅ **是，應該建立專用 Skill**

### 現況分析

**現有 Skills 清單：**
1. `technical-deep-dive.md` - 阻抗匹配、訊號路徑技術驗證
2. `equipment-optimizer.md` - 功能重疊檢測、使用率優化
3. `guitar-pedal-pairing.md` - 吉他與效果器配對分析
4. `inventory-manager.md` - 庫存管理
5. `budget-analyzer.md` - 預算分析
6. `implementation-planner.md` - 實作規劃

**缺失：**
- ❌ 沒有專門生成「使用範例文件」的 Skill
- ❌ 現有 Skills 都聚焦於「分析」而非「實用範例生成」

---

### 解決方案：✅ 已建立

**新 Skill：`usage-examples-generator.md`**

**核心功能：**
1. 解析 YAML 技術規格
2. 整合 Research 文件資訊
3. 生成控制介面完整說明
4. 創建實際使用範例（針對不同音樂風格）
5. 提供設定建議與故障排除

**與現有 Skills 的差異：**

| Skill | 定位 | 輸出 | 目標用戶 |
|-------|------|------|---------|
| **Technical Deep-Dive** | 技術分析 | 阻抗匹配報告、訊號路徑驗證 | 進階玩家 |
| **Equipment Optimizer** | 設備優化 | 功能重疊分析、替換建議 | 玩家 + 預算考量 |
| **Usage Examples Generator** | 實用指南 | 旋鈕說明、範例設定、故障排除 | **所有用戶（尤其初學者）** |

**優勢：**
- ✅ 填補「技術規格 → 實際應用」之間的鴻溝
- ✅ 將 YAML 冷冰冰的數據轉化為可操作的範例
- ✅ 針對用戶的音樂風格客製化範例

---

## 問題 2: 範例文件內容除了範例之外應該包含什麼？

### 回答：範例文件應包含以下**完整章節**

### **必要章節（Priority 1）**

#### 1. **控制介面完整說明** ⭐⭐⭐
你提到「至少要有所有旋鈕、按鈕的功能說明」，這是**核心需求**。

**應包含的資訊：**
- **旋鈕/按鈕名稱**
- **位置** (在面板上的位置描述)
- **功能** (這個控制項做什麼)
- **調整範圍** (如 20ms-2000ms, 0-100%)
- **調整影響** (順時針/逆時針、向上/向下的效果)
- **使用技巧** (不同情境的設定建議)

**範例格式：**
```markdown
#### **Delay Time (×2) - 延遲時間**
- **位置:** 雙旋鈕（Delay A 和 Delay B 各一個）
- **功能:** 設定延遲音重複的時間間隔
- **範圍:** 待手冊確認（典型數位延遲為 20ms ~ 2000ms）
- **調整影響:**
  - **順時針旋轉** → 延遲時間變長（節奏變慢）
  - **逆時針旋轉** → 延遲時間變短（節奏變快）
- **使用技巧:**
  - **短延遲 (20-120ms)**: Slap Back、增加厚度
  - **中延遲 (120-400ms)**: 節奏延遲、配合歌曲速度
  - **長延遲 (400ms+)**: Ambient、音景創造
```

---

#### 2. **實際使用範例** ⭐⭐⭐

**每個範例應包含：**
- **範例名稱** (如「立體聲 Ping-Pong Delay」)
- **適用音樂風格** (Jazz, Post Rock, etc.)
- **參數設定表格** (清楚列出所有旋鈕設定值)
- **效果描述** (實際聽到什麼聲音)
- **適合場景** (什麼時候使用)

**範例數量建議：**
- **最少 5 個範例**
- **涵蓋用戶的主要音樂風格**
- **包含基礎 + 進階範例**

**範例格式：**
```markdown
### **範例 1：立體聲 Ping-Pong Delay（乒乓延遲）**

**音樂風格**: Post Rock, Ambient, Neo Soul

**設定**:
| 參數 | Delay A | Delay B |
|------|---------|---------|
| **Time** | 400ms（四分音符） | 600ms（附點四分音符） |
| **Feedback** | 3次重複 | 3次重複 |
| **Pan/Output** | Left（左聲道） | Right（右聲道） |

**全局設定**:
- **Mix**: 40-50%
- **Modulation Depth**: 低（10-20%）

**效果**:
- 延遲音在左右聲道交替出現（Ping-Pong 效果）
- 創造寬廣的立體聲空間感

**適合場景**:
- Clean Tone Arpeggios
- Ambient Lead Guitar
```

---

#### 3. **音樂風格設定指南** ⭐⭐

根據用戶常彈的音樂風格，提供快速設定參考。

**範例格式：**
```markdown
### **Jazz**

**典型設定**:
- Delay Time: 120-300ms（短至中延遲）
- Feedback: 1-3次（不過度重複）
- Mix: 20-30%（細膩）
- Modulation: 10-20%（細微）

**關鍵要點**:
- Jazz 需要保持清晰，延遲不宜過長
- 使用 Slap Back 增加厚度而非空間感
```

---

### **建議章節（Priority 2）**

#### 4. **故障排除** ⭐⭐

列出 5-10 個常見問題及解決方案。

**範例格式：**
```markdown
**問題：延遲音過於混濁**
- **解決方案**: 削減 **EQ Low** -2 至 -4dB

**問題：延遲音太亮、刺耳**
- **解決方案**: 削減 **EQ High** -2 至 -3dB
```

---

#### 5. **進階技巧** ⭐⭐

展示效果器的進階應用。

**範例格式：**
```markdown
### **同一首歌內切換模式**

**場景範例：Post Rock 歌曲結構**

| 歌曲段落 | 模式 | 預設設定 | 效果 |
|---------|------|---------|------|
| **Verse（主歌）** | Parallel | Mix 30% | 簡單清晰 |
| **Chorus（副歌）** | Parallel | Mix 50% | 更豐富 |
| **Bridge** | Series | Mix 70-80% | 瀑布延遲 |

**操作方式**:
- 使用 **MIDI Program Change** 快速切換
- 利用 **Trail Function** 讓切換更自然
```

---

#### 6. **與用戶設備搭配** ⭐

根據用戶擁有的吉他、音箱提供客製化建議。

**範例格式：**
```markdown
### **與 ESP Throbber CTM 搭配（PAF 8.7k）**

**建議設定**:
- PAF 被動拾音器輸出較低，可能需要提升 Input Gain
- 延遲音可稍微提升高頻（PAF 偏溫暖）

### **與 Tone King Imperial MKII FX Loop 搭配**

**建議設定**:
- FX Loop 為 Stereo，充分利用 FF-1Y 的立體聲輸出
- 使用 Parallel 模式創造寬廣空間感
```

---

### **可選章節（Priority 3）**

#### 7. **與其他效果器搭配**

如何與用戶已有的其他效果器搭配使用。

---

#### 8. **Preset 管理策略**

如果效果器支援預設功能（如 FF-1Y 的 128 預設），提供預設庫規劃建議。

---

#### 9. **初學者 vs 進階使用者指南**

分別針對不同經驗等級提供建議。

---

### **章節優先順序總結**

| 優先級 | 章節 | 必要性 | 原因 |
|-------|------|--------|------|
| **P1** | 控制介面完整說明 | ⭐⭐⭐ | 用戶明確需求 |
| **P1** | 實際使用範例 | ⭐⭐⭐ | 文件核心價值 |
| **P1** | 音樂風格設定指南 | ⭐⭐⭐ | 客製化建議 |
| **P2** | 故障排除 | ⭐⭐ | 解決實際問題 |
| **P2** | 進階技巧 | ⭐⭐ | 提升使用深度 |
| **P2** | 與用戶設備搭配 | ⭐⭐ | 個人化建議 |
| **P3** | 與其他效果器搭配 | ⭐ | 進階應用 |
| **P3** | Preset 管理策略 | ⭐ | 特定效果器需要 |
| **P3** | 初學者 vs 進階指南 | ⭐ | Nice to have |

---

## 問題 3: 現行 Research Skill/Agent 收集到的資訊是否足夠建立範例文件？

### 回答：⚠️ **部分足夠，但需要增強**

---

### 現況評估

#### ✅ **現行 Research 已收集的資訊（足夠）**

從 `ff1y.yaml` 和 `compressor_eq_spatial_effects_technical_data.md` 來看：

| 資訊類別 | YAML 覆蓋度 | Research MD 覆蓋度 | 足夠建立範例文件？ |
|---------|------------|-------------------|-----------------|
| **基本資訊** | ✅ 完整 | ✅ 完整 | ✅ 足夠 |
| **技術規格** | ✅ 完整 | ✅ 完整 | ✅ 足夠 |
| **創新功能** | ✅ 完整 | ✅ 完整 | ✅ 足夠 |
| **音色特性** | ✅ 完整 | ✅ 完整 | ✅ 足夠 |
| **使用建議** | ✅ 有 | ✅ 有 | ✅ 足夠（可轉換為範例） |
| **音樂風格** | ✅ 列表 | ✅ 列表 | ✅ 足夠 |
| **與其他設備比較** | ✅ 有（FT-1Y） | ✅ 有 | ✅ 足夠 |

---

#### ❌ **現行 Research 缺少的資訊（不足夠）**

| 資訊類別 | YAML 狀態 | Research MD 狀態 | 影響 | 優先級 |
|---------|----------|-----------------|------|--------|
| **控制項詳細參數** | ⚠️ 只有名稱列表 | ❌ 無 | 無法寫出「調整範圍」「調整影響」 | **P1 高** |
| **控制項位置** | ❌ 無 | ❌ 無 | 無法描述「旋鈕在面板上的位置」 | P2 中 |
| **具體參數值範圍** | ⚠️ 部分待確認 | ❌ 無 | 無法提供精確設定建議 | **P1 高** |
| **實際音色範例描述** | ⚠️ 抽象描述 | ✅ 有部分 | 難以寫出「實際聽到的效果」 | P2 中 |
| **常見問題與解決方案** | ❌ 無 | ⚠️ 只有 pros/cons | 無法生成完整故障排除 | P2 中 |
| **面板佈局圖** | ❌ 無 | ❌ 無 | 無法提供視覺化指引 | P3 低 |

---

### 具體問題舉例

#### 問題 1: 控制項詳細參數不足

**現狀（ff1y.yaml Line 102-111）：**
```yaml
controls:
  main_controls:
    - "Delay Time (×2 for dual delays)"
    - "Feedback (×2)"
    - "Mix"
    - "EQ (3-band)"
    - "Modulation controls"
    - "Routing select"
    - "Soft Clipping control"
```

**問題：**
- ❌ 只有控制項名稱
- ❌ 沒有調整範圍（如 Delay Time: 20ms-2000ms?）
- ❌ 沒有控制項類型（旋鈕 or 開關？）
- ❌ 沒有位置資訊（面板左側 or 右側？）

**影響：**
生成的範例文件中，所有控制項說明都會變成：
```markdown
#### **Delay Time**
- **範圍:** 待手冊確認（典型數位延遲為 20ms ~ 2000ms）
```

---

#### 問題 2: 具體參數值缺失

**現狀（ff1y.yaml Line 197-223）：**
```yaml
usage_tips:
  dual_delay_routing:
    parallel:
      description: "兩組延遲並聯運作"
      use_case: "創造豐富的立體聲延遲效果"
    series:
      description: "兩組延遲串聯運作"
      use_case: "創造複雜的疊加延遲效果"

  soft_clipping_usage:
    steps:
      - "啟用 Soft Clipping"
      - "為延遲訊號添加諧波"
      - "創造更溫暖、更具類比感的延遲音色"
```

**問題：**
- ❌ 沒有具體參數值（如 Delay Time 設多少？）
- ❌ 沒有範例場景（什麼歌曲？什麼風格？）
- ⚠️ 只有抽象描述，無法直接轉換為「可操作的範例」

**影響：**
需要**推測**合理的參數值，或標註為「建議範例設定」。

---

### 改進建議

#### 建議 1: 增強 Research Agent 的資料收集 ⭐⭐⭐

**修改 `1_pedal-researcher.md` 的 Step 4: Web Search**

**新增搜尋目標：**
```yaml
Step 4.4: 搜尋控制項詳細資訊

Search Queries:
  - "[Brand] [Model] manual PDF"
  - "[Brand] [Model] controls explanation"
  - "[Brand] [Model] knob functions"

提取資訊:
  - 每個旋鈕/開關的調整範圍
  - 控制項位置（從產品圖片推測）
  - 特殊控制項的功能說明（如 Bite Control, Tilt EQ）

優先來源:
  1. 官方使用手冊 PDF
  2. 官方產品頁面的控制項說明
  3. 詳細評測文章（Premier Guitar 等）
```

**新增搜尋目標：**
```yaml
Step 4.5: 搜尋實際使用範例

Search Queries:
  - "[Brand] [Model] settings examples"
  - "[Brand] [Model] how to use"
  - "[Brand] [Model] best settings for [style]"

提取資訊:
  - 評測者提供的具體參數設定
  - 不同音樂風格的推薦設定
  - 常見問題與解決方案（論壇、評論）

優先來源:
  1. YouTube 評測影片（觀察旋鈕位置）
  2. 部落格詳細評測
  3. The Gear Page 等論壇的用戶設定分享
```

---

#### 建議 2: 增強 YAML Schema ⭐⭐⭐

**修改 YAML 範本，增加控制項詳細欄位：**

```yaml
# 現行（不足）
controls:
  main_controls:
    - "Delay Time (×2 for dual delays)"
    - "Feedback (×2)"

# 建議改為（完整）
controls:
  delay_time_a:
    name: "Delay Time A"
    type: "rotary_knob"  # rotary_knob, toggle_switch, push_button
    position: "top_left"
    range:
      min: "20ms"
      max: "2000ms"
      unit: "milliseconds"
    function: "設定 Delay A 的延遲時間"
    impact:
      clockwise: "延遲時間變長（節奏變慢）"
      counter_clockwise: "延遲時間變短（節奏變快）"
    notes: "可透過 Tap Tempo 快速設定"

  delay_time_b:
    name: "Delay Time B"
    type: "rotary_knob"
    position: "top_right"
    range:
      min: "20ms"
      max: "2000ms"
      unit: "milliseconds"
    function: "設定 Delay B 的延遲時間"
    impact:
      clockwise: "延遲時間變長（節奏變慢）"
      counter_clockwise: "延遲時間變短（節奏變快）"

  # ... 其他控制項
```

**優點：**
- ✅ 可直接轉換為範例文件的「控制介面說明」章節
- ✅ 結構化資料易於 AI 處理
- ✅ 明確標註待確認欄位（如 `range: "待手冊確認"`）

---

#### 建議 3: 增強 usage_tips 結構 ⭐⭐

**修改 YAML 範本，增加具體範例：**

```yaml
# 現行（抽象）
usage_tips:
  dual_delay_routing:
    parallel:
      description: "兩組延遲並聯運作"
      use_case: "創造豐富的立體聲延遲效果"

# 建議改為（具體）
usage_examples:
  - example_id: "parallel_ping_pong"
    name: "立體聲 Ping-Pong Delay"
    music_styles: ["Post Rock", "Ambient", "Neo Soul"]
    routing_mode: "Parallel"

    settings:
      delay_a:
        time: "400ms"
        feedback: "3 repeats"
        pan: "Left"
      delay_b:
        time: "600ms"
        feedback: "3 repeats"
        pan: "Right"
      mix: "40-50%"
      modulation_depth: "10-20%"

    effect_description: |
      延遲音在左右聲道交替出現（Ping-Pong 效果），
      創造寬廣的立體聲空間感。

    suitable_scenarios:
      - "Clean Tone Arpeggios"
      - "Ambient Lead Guitar"
      - "Post Rock Clean Riffs"

  - example_id: "series_tape_echo"
    name: "磁帶回音模擬"
    music_styles: ["Blues", "Classic Rock", "Neo Soul"]
    routing_mode: "Series"

    settings:
      delay_a:
        time: "350ms"
        feedback: "4 repeats"
        eq_high: "-2dB"
      delay_b:
        time: "350ms"
        feedback: "3 repeats"
        eq_high: "-4dB"
      mix: "35%"
      modulation_depth: "30-40%"
      soft_clipping: "35%"

    effect_description: |
      延遲音經過兩次處理，每次都損失高頻，
      創造類比磁帶回音的漸暗效果。

    suitable_scenarios:
      - "Blues Lead Solo"
      - "Classic Rock Rhythm"
      - "Neo Soul Vintage Tones"
```

**優點：**
- ✅ 可直接轉換為範例文件的「實際使用範例」章節
- ✅ 包含具體參數值
- ✅ 包含音樂風格與應用場景

---

#### 建議 4: 增加「待手冊確認」機制 ⭐⭐

**在 Research Agent 中增加驗證步驟：**

```yaml
Step 6: 資料完整度驗證

檢查 YAML 中的關鍵欄位:
  - controls (是否有詳細參數？)
  - usage_examples (是否有具體設定值？)
  - 特殊功能說明 (是否清楚？)

if 資料不完整:
  標註為「待手冊確認」
  提供合理推測值（基於同類型效果器）

  範例:
  ```yaml
  delay_time_a:
    range:
      min: "20ms"  # 待手冊確認，典型數位延遲範圍
      max: "2000ms"  # 待手冊確認
      data_source: "inferred_from_pedal_type"
  ```
```

---

### 改進後的工作流程

```
User: "研究 Free the Tone FF-1Y"

┌─────────────────────────────────────────┐
│ Step 1-3: 基本資訊收集（現有流程）          │
│ - 基本資訊                                │
│ - 技術規格                                │
│ - 創新功能                                │
└─────────────────────────────────────────┘
              ↓
┌─────────────────────────────────────────┐
│ Step 4.4: 控制項詳細資訊收集（新增）        │
│ - 搜尋官方手冊 PDF                         │
│ - 提取每個旋鈕的調整範圍                    │
│ - 從產品圖片推測控制項位置                  │
└─────────────────────────────────────────┘
              ↓
┌─────────────────────────────────────────┐
│ Step 4.5: 使用範例收集（新增）             │
│ - 搜尋 YouTube 評測（觀察旋鈕設定）         │
│ - 搜尋論壇用戶分享的設定                   │
│ - 提取不同風格的具體參數值                 │
└─────────────────────────────────────────┘
              ↓
┌─────────────────────────────────────────┐
│ Step 6: 資料完整度驗證（新增）             │
│ - 檢查控制項是否有詳細參數                 │
│ - 檢查是否有具體使用範例                   │
│ - 標註「待手冊確認」欄位                   │
└─────────────────────────────────────────┘
              ↓
┌─────────────────────────────────────────┐
│ Step 7: 生成 YAML + MD（現有流程）         │
│ - 使用新 Schema（包含詳細控制項資訊）      │
│ - 使用新 usage_examples 結構              │
└─────────────────────────────────────────┘
              ↓
┌─────────────────────────────────────────┐
│ Step 8: 生成使用範例文件（新增）           │
│ - 呼叫 Usage Examples Generator Skill    │
│ - 自動轉換 YAML 為使用範例文件             │
│ - 標註待確認資訊                          │
└─────────────────────────────────────────┘
              ↓
┌─────────────────────────────────────────┐
│ 輸出                                     │
│ - ff1y.yaml (完整技術規格)                │
│ - research_report.md (研究報告)          │
│ - ff1y_examples.md (使用範例文件) ✨ 新   │
└─────────────────────────────────────────┘
```

---

## 總結與行動建議

### ✅ 問題 1: 是否建立專用 Skill？

**答案：是**
已建立 `usage-examples-generator.md` Skill。

---

### ✅ 問題 2: 範例文件應包含什麼？

**必要章節（P1）：**
1. 控制介面完整說明（所有旋鈕、按鈕的詳細說明）⭐⭐⭐
2. 實際使用範例（至少 5 個，含參數表格）⭐⭐⭐
3. 音樂風格設定指南⭐⭐⭐

**建議章節（P2）：**
4. 故障排除（5-10 個問題）⭐⭐
5. 進階技巧⭐⭐
6. 與用戶設備搭配⭐⭐

**可選章節（P3）：**
7. 與其他效果器搭配⭐
8. Preset 管理策略⭐

---

### ⚠️ 問題 3: 現行 Research 是否足夠？

**答案：部分足夠，需要增強**

**足夠的資訊：**
- ✅ 基本資訊、技術規格、創新功能
- ✅ 音色特性、音樂風格列表
- ✅ 使用建議（可轉換為範例）

**不足的資訊：**
- ❌ 控制項詳細參數（調整範圍、位置）**← P1 優先改進**
- ❌ 具體使用範例（參數值、設定表）**← P1 優先改進**
- ❌ 常見問題與解決方案

**改進建議優先順序：**

| 優先級 | 改進項目 | 影響 | 工作量 |
|-------|---------|------|--------|
| **P1** | 增強 YAML Schema（控制項詳細欄位） | 高 | 中 |
| **P1** | 增強 Research Agent（搜尋控制項資訊） | 高 | 中 |
| **P2** | 增強 YAML Schema（usage_examples 結構） | 中 | 中 |
| **P2** | 增強 Research Agent（搜尋實際範例） | 中 | 高 |
| **P3** | 增加資料完整度驗證機制 | 中 | 低 |

---

## 下一步行動

### 立即可執行（已完成）：
- ✅ 建立 `usage-examples-generator.md` Skill
- ✅ 生成 `ff1y_examples.md` 範例文件（展示輸出格式）

### 短期（建議 1-2 天內）：
1. **修改 YAML Schema** - 增加控制項詳細欄位
2. **修改 Research Agent** - 增加控制項資訊搜尋步驟

### 中期（建議 1 週內）：
3. **重新研究 FF-1Y** - 使用新流程，生成更完整的 YAML
4. **更新範例文件** - 根據新 YAML 重新生成

### 長期（持續優化）：
5. 為其他效果器生成使用範例文件
6. 收集用戶反饋，持續改進範例品質

---

**文件完成日期:** 2026-01-11
**下次檢視:** 新 Research Agent 修改完成後
