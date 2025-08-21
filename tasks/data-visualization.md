<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 數據視覺化 (Data Visualization)

## Purpose

此任務旨在協助進行數據視覺化，例如建議圖表類型或生成圖表描述，幫助使用者將複雜數據轉化為直觀、易懂的視覺形式，提升數據溝通效率。

## Inputs

- **`raw_data`**: 需要視覺化的原始數據集。
- **`visualization_goal`**: 視覺化的目的（例如：展示趨勢、比較數據、揭示分佈）。
- **`target_audience`** (Optional): 視覺化的目標受眾。
- **`preferred_chart_types`** (Optional): 偏好的圖表類型（例如：柱狀圖、折線圖、圓餅圖、散點圖）。

## Process

### 1. 理解數據與視覺化目標

- 審閱 `raw_data`，理解數據的結構、類型和潛在關係。
- 明確 `visualization_goal`，確定視覺化需要傳達的核心訊息。
- 考慮 `target_audience` 的數據理解能力和偏好。

### 2. 建議圖表類型

- 根據 `raw_data` 的特性和 `visualization_goal`，建議最適合的圖表類型。
- 如果提供了 `preferred_chart_types`，則優先考慮。
- 解釋為什麼推薦某種圖表類型（例如：折線圖適合展示趨勢，柱狀圖適合比較）。

### 3. 生成圖表描述或範例

- 如果無法直接生成圖表，則生成詳細的圖表描述，包括：
    - 圖表標題。
    - X 軸和 Y 軸的標籤。
    - 數據系列。
    - 圖例。
    - 關鍵數據點或趨勢的標註。
- 可以提供程式碼範例（例如：Python 的 Matplotlib/Seaborn、JavaScript 的 D3.js）來生成圖表。

### 4. 解釋視覺化洞察

- 解釋圖表所揭示的關鍵洞察、趨勢或模式。
- 強調視覺化如何支持 `visualization_goal`。

## Outputs

- **`visualization_suggestion`**: 建議的圖表類型和其理由。
- **`chart_description`**: 詳細的圖表描述，可用於手動繪製或程式生成。
- **** (Optional): 生成圖表的程式碼範例。
- **`key_insights_from_chart`** (Optional): 從視覺化中提取的關鍵洞察。

## Key Principles

- **清晰性**: 視覺化應清晰明瞭，易於理解。
- **準確性**: 圖表應準確反映數據，不誤導讀者。
- **目的導向**: 視覺化應服務於特定目的，傳達核心訊息。
- **美觀性**: 在保證清晰和準確的前提下，追求視覺上的美觀。
