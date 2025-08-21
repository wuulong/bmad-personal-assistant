<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 每日活動總結 (Summarize Daily Activities)

## Purpose

此任務旨在每日總結與個人助理的互動、已完成任務和待辦事項，幫助使用者快速回顧一天的工作和進度。

## Inputs

- **`interaction_log`**: 當日與個人助理的所有對話和互動記錄。
- **`completed_tasks_list`**: 當日已標記為完成的任務清單。
- **`pending_todo_list`**: 當日尚未完成的待辦事項清單。

## Process

### 1. 收集當日數據

- 從 `interaction_log` 中提取關鍵對話點、決策和指令。
- 匯總 `completed_tasks_list` 中的所有已完成任務。
- 匯總 `pending_todo_list` 中的所有未完成待辦事項。

### 2. 提煉核心資訊

- 識別互動中的重要主題和模式。
- 總結每個已完成任務的成果。
- 列出每個未完成待辦事項的當前狀態和預計進度。

### 3. 生成總結報告

- 以清晰、簡潔的格式呈現總結內容。
- 報告應包含：
    - 當日主要互動亮點。
    - 已完成任務的清單。
    - 待辦事項的更新狀態。
    - 任何需要使用者特別關注的事項。

## Outputs

- **`daily_summary_report`**: 每日活動的總結報告，以 Markdown 或其他易讀格式呈現。

## Key Principles

- **簡潔明瞭**: 報告內容應精煉，突出重點。
- **全面性**: 涵蓋所有重要互動和任務狀態。
- **易讀性**: 採用清晰的標題和列表，方便使用者快速瀏覽。
- **定時性**: 確保每日在固定時間生成和提供報告。
