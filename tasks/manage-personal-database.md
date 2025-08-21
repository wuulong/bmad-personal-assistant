<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 管理個人資料庫 (Manage Personal Database)

## Purpose

此任務旨在協助使用者建構、更新和管理個人的資料庫（例如：筆記資料庫、專案資料庫、聯絡人資料庫），以實現資訊的系統化儲存、高效檢索和持續維護。

## Inputs

- **`database_name`**: 需要管理或建立的資料庫名稱。
- **`operation_type`**: 資料庫操作類型（例如：建立、新增記錄、更新記錄、查詢、刪除記錄）。
- **`record_content`** (Optional): 新增或更新記錄的內容。
- **`query_criteria`** (Optional): 查詢記錄的條件。
- **`database_schema`** (Optional): 資料庫的結構定義（例如：表格、欄位）。

## Process

### 1. 理解資料庫需求

- 根據 `database_name` 和 `operation_type`，明確使用者的資料庫管理需求。
- 如果是建立新資料庫，則根據 `database_schema` 或使用者描述，設計資料庫結構。

### 2. 執行資料庫操作

- **建立**: 根據定義建立新的資料庫。
- **新增記錄**: 將 `record_content` 添加到指定資料庫中。
- **更新記錄**: 根據 `query_criteria` 找到記錄，並用 `record_content` 更新。
- **查詢**: 根據 `query_criteria` 從資料庫中檢索記錄。
- **刪除記錄**: 根據 `query_criteria` 從資料庫中刪除記錄。

### 3. 處理數據完整性與一致性

- 確保所有操作都符合資料庫的完整性約束。
- 處理數據衝突或重複。

### 4. 提供操作結果

- 向使用者回報操作的結果，例如：
    - 新增記錄的 ID。
    - 查詢到的記錄清單。
    - 更新或刪除的記錄數量。
    - 任何錯誤訊息。

## Outputs

- **`operation_result`**: 資料庫操作的結果，可以是查詢結果、操作狀態或錯誤訊息。
- **`updated_database_state`** (Optional): 操作後資料庫的最新狀態（例如：記錄數量）。

## Key Principles

- **數據安全**: 確保資料庫內容的安全性和隱私。
- **高效檢索**: 設計資料庫結構以支持快速查詢。
- **易於維護**: 確保資料庫結構清晰，方便後續的更新和擴展。
- **使用者控制**: 所有資料庫操作都應在使用者明確指令下進行。
