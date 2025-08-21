<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 整理對話 (Organize Conversation)

```yaml
name: 整理對話
id: organize-conversation
description: 整理與使用者的對話內容，提取關鍵資訊、決策點和待辦事項。
parameters:
  # No specific parameters defined yet, will be added later if needed
```

## 產製對話紀錄的方法

當需要將聊天室歷史記錄整理成對話紀錄時，可遵循以下步驟：

1.  **讀取對話歷史檔案**：
    *   使用 `read_file` 工具讀取包含對話歷史的 JSON 格式檔案（例如：`tmp/checkpoint-XXXXXX.json`）。

2.  **解析與提取 Q&A**：
    *   解析讀取到的 JSON 內容，該內容通常是一個包含多個對話回合（turn）的列表。
    *   每個回合包含 `role` (user/model) 和 `parts`。從 `parts` 中提取 `text` 內容。
    *   如果模型的回應包含 `functionCall` 或 `functionResponse`，也應將其內容一併提取並納入回答中。

3.  **格式化 Q&A 紀錄**：
    *   將提取的用戶提問 (Q) 和模型回答 (A) 按照 `M::備註\nQ::提問內容\nA::你的回答` 的格式進行組織。
    *   `M::備註` 部分可用於添加對話的整體說明或特定回合的註解。

4.  **儲存格式化後的紀錄**：
    *   將格式化後的 Q&A 內容寫入一個新的 Markdown 檔案。
    *   檔案命名應遵循 `tmp/note_{YYMMDD}-{隨機五位數字}.md` 的臨時命名規範。

5.  **移動與重新命名檔案**：
    *   將臨時儲存的對話紀錄檔案移動到知識庫中對應的目錄（例如：`KnowledgeBase/CommunicationAndCollaboration/ConversationRecords/`）。
    *   將檔案重新命名為有意義的名稱，並在前面加上日期（例如：`YYYY-MM-DD_有意義的檔名.md`）。
