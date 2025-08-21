<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 管理行程 (Manage Schedule)

## Purpose

此任務旨在協助使用者管理個人或專業行程，包括會議、約會和活動，確保時間高效利用，避免衝突。

## Inputs

- **`event_details`**: 需要添加到行程中的事件詳細資訊（例如：事件名稱、日期、時間、地點、參與者）。
- **`operation_type`**: 行程操作類型（例如：新增、更新、刪除、查詢）。
- **`query_criteria`** (Optional): 查詢行程的條件（例如：日期範圍、事件名稱）。

## Process

### 1. 理解行程需求

- 根據 `operation_type`，明確使用者對行程管理的需求。
- 如果是新增事件，則解析 `event_details`。
- 如果是查詢、更新或刪除，則解析 `query_criteria`。

### 2. 檢查時間衝突

- 在新增或更新事件時，檢查與現有行程是否存在時間衝突。
- 如果存在衝突，則向使用者發出提醒並建議解決方案。

### 3. 執行行程操作

- **新增**: 將新事件添加到行程中。
- **更新**: 根據 `query_criteria` 找到事件，並用 `event_details` 更新。
- **刪除**: 根據 `query_criteria` 從行程中刪除事件。
- **查詢**: 根據 `query_criteria` 從行程中檢索事件。

### 4. 提供操作結果

- 向使用者回報操作的結果，例如：
    - 新增事件的確認。
    - 查詢到的事件清單。
    - 更新或刪除的事件確認。
    - 任何錯誤訊息或衝突提醒。

## Outputs

- **`schedule_update_confirmation`**: 行程操作的確認訊息。
- **`retrieved_events`**: 查詢操作返回的事件清單。
- **`conflict_alert`** (Optional): 如果存在時間衝突，發出的警報。

## Key Principles

- **準確性**: 確保行程資訊的準確性。
- **即時性**: 確保行程更新的即時性。
- **防衝突**: 盡可能避免時間衝突。
- **使用者控制**: 所有行程操作都應在使用者明確指令下進行。
