<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 分類資訊 (Categorize Information)

## Purpose

此任務旨在將非結構化資訊分類到預設或建議的類別中，幫助使用者建立清晰的資訊結構，方便管理和檢索。

## Inputs

- **`information_content`**: 需要分類的資訊內容（例如：筆記、文章、網頁內容、文件）。
- **`existing_categories`** (Optional): 使用者已有的分類體系或標籤清單。
- **`categorization_goal`** (Optional): 分類的具體目的或使用場景。

## Process

### 1. 理解資訊內容

- 仔細閱讀 `information_content`，理解其主題、關鍵概念和核心內容。

### 2. 識別分類依據

- 根據 `categorization_goal` 和 `existing_categories`，識別適合該資訊的分類維度或標籤。
- 如果沒有提供現有類別，則根據內容自動建議合適的分類。

### 3. 執行分類

- 將資訊內容歸入一個或多個最相關的類別。
- 確保分類的準確性和一致性。

### 4. 呈現分類結果

- 以清晰的方式呈現分類結果，例如：
    - 建議的類別標籤清單。
    - 資訊內容與類別的對應關係。

## Outputs

- **`categorized_info`**: 包含原始資訊內容和建議分類標籤的結構化數據。
- **`suggested_new_categories`** (Optional): 如果現有類別不夠用，建議新增的類別。

## Key Principles

- **相關性**: 分類應與資訊內容高度相關。
- **一致性**: 確保在不同資訊之間應用相同的分類標準。
- **靈活性**: 允許資訊歸入多個類別，以反映其多維度屬性。
- **易用性**: 分類結果應方便使用者理解和後續檢索。
