<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 設定提醒 (Set Reminders)

## Purpose

此任務旨在協助使用者設定和管理各種事件或任務的提醒，確保使用者不會錯過重要事項，提升時間管理效率。

## Inputs

- **`reminder_content`**: 提醒的具體內容（例如：會議提醒、繳費提醒、生日提醒）。
- **`reminder_time`**: 提醒的時間點（例如：具體日期時間、相對時間如「30分鐘後」）。
- **`recurrence`** (Optional): 提醒的重複頻率（例如：每日、每週、每月、每年）。
- **`notification_method`** (Optional): 偏好的提醒方式（例如：彈出通知、郵件、訊息）。

## Process

### 1. 理解提醒需求

- 解析 `reminder_content` 和 `reminder_time`，明確提醒的具體內容和觸發時間。
- 考慮 `recurrence` 和 `notification_method`。

### 2. 建立提醒

- 根據使用者提供的資訊，在提醒系統中建立新的提醒。
- 確保提醒的準確性和可觸發性。

### 3. 管理提醒

- 允許使用者查詢、更新或刪除已設定的提醒。
- 確保提醒在指定時間點準確觸發。

### 4. 發送通知

- 在提醒時間到達時，透過 `notification_method` 向使用者發送通知。

## Outputs

- **`reminder_confirmation`**: 提醒設定成功的確認訊息。
- **`triggered_notification`**: 在指定時間點發送的提醒通知。

## Key Principles

- **準確性**: 確保提醒時間和內容的準確性。
- **及時性**: 提醒應在正確的時間點觸發。
- **多樣性**: 提供多種提醒方式以適應不同場景。
- **使用者控制**: 允許使用者完全控制提醒的設定和管理。
