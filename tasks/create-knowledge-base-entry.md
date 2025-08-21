<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 建立知識庫條目 (Create Knowledge Base Entry)

## Purpose

此任務旨在根據提供的資訊，在個人知識庫中建立新的條目或更新現有條目，以系統化地儲存和管理個人知識。

## Inputs

- **`entry_content`**: 知識庫條目的主要內容（例如：筆記、摘要、概念解釋、操作步驟）。
- **`entry_title`**: 知識庫條目的標題。
- **`tags`** (Optional): 用於分類和檢索的關鍵字或標籤清單。
- **`related_entries`** (Optional): 與此條目相關的其他知識庫條目。
- **`update_existing`** (Optional): 布林值，指示是否更新現有條目（如果存在）。

## Process

### 1. 識別條目類型與結構

- 根據 `entry_content` 和 `entry_title`，判斷條目的性質（概念、流程、事實等）。
- 確定條目在知識庫中的最佳結構和位置。

### 2. 檢查現有條目

- 如果 `update_existing` 為真，則搜尋知識庫中是否存在標題或內容相似的現有條目。
- 如果找到，則準備更新。

### 3. 格式化條目內容

- 將 `entry_content` 格式化為知識庫的標準格式（例如：Markdown、富文本）。
- 確保內容清晰、簡潔、易於閱讀。

### 4. 添加元數據與關聯

- 添加 `entry_title`、`tags` 和 `related_entries` 等元數據。
- 建立與其他相關條目的連結。

### 5. 儲存或更新條目

- 如果是新條目，則將其儲存到知識庫中。
- 如果是更新現有條目，則覆蓋或合併舊內容。

## Outputs

- **`knowledge_base_entry_path`**: 建立或更新的知識庫條目的儲存路徑或唯一識別符。
- **`status_message`**: 指示操作成功或失敗的訊息。

## Key Principles

- **唯一性**: 確保每個知識點都有其獨立的條目。
- **可檢索性**: 透過標籤和關聯，方便快速檢索。
- **一致性**: 保持知識庫條目格式和風格的一致性。
- **可擴展性**: 知識庫應能隨著新知識的增加而持續成長。
