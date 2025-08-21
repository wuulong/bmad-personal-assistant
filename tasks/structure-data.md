<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 結構化資料 (Structure Data)

## Purpose

此任務旨在將非結構化資料轉換為結構化格式（例如：從文字中提取資訊並轉換為表格、JSON 或 YAML 格式），以便於數據的儲存、分析和利用。

## Inputs

- **`unstructured_data`**: 需要結構化的非結構化數據內容（例如：自由文本、筆記、網頁內容、掃描文件）。
- **`target_format`**: 期望的結構化格式（例如：表格、JSON、YAML）。
- **`schema_definition`** (Optional): 期望的數據結構定義（例如：JSON Schema、表格列名）。

## Process

### 1. 理解非結構化數據

- 仔細閱讀 `unstructured_data`，理解其內容、語義和潛在的結構模式。
- 識別數據中包含的實體、屬性、關係和事件。

### 2. 設計或應用數據結構

- 如果提供了 `schema_definition`，則按照定義進行結構化。
- 如果未提供，則根據數據內容和 `target_format`，自動設計一個合理的數據結構。

### 3. 提取與轉換數據

- 從非結構化數據中精確提取所需資訊。
- 將提取的資訊轉換為 `target_format`。
- 處理數據中的歧義、不一致或缺失值。

### 4. 驗證結構化數據

- 檢查結構化數據是否符合 `target_format` 和 `schema_definition`。
- 確保數據的完整性和準確性。

## Outputs

- **`structured_data_output`**: 轉換後的結構化數據，以指定格式呈現。
- **`conversion_report`** (Optional): 轉換過程的報告，包括任何遇到的問題或假設。

## Key Principles

- **精確性**: 確保數據提取和轉換的準確性。
- **完整性**: 盡可能保留原始數據中的所有相關資訊。
- **一致性**: 確保結構化數據的格式和內容一致。
- **可用性**: 結構化數據應易於後續的儲存、查詢和分析。
