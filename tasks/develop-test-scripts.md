<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 開發測試腳本 (Develop Test Scripts)

## Purpose

此任務旨在根據需求開發自動化測試腳本，以驗證軟體功能、性能或安全性，提高測試效率和準確性。

## Inputs

- **`test_requirements`**: 測試腳本的需求描述（例如：測試目標、測試範圍、測試場景、預期結果）。
- **`system_under_test_info`**: 被測系統的相關資訊（例如：API 文件、UI 截圖、程式碼片段）。
- **`testing_framework_preference`** (Optional): 偏好的測試框架或語言（例如：Selenium、Cypress、Pytest、Junit）。

## Process

### 1. 理解測試需求

- 深入分析 `test_requirements`，將其分解為可執行的測試步驟。
- 明確測試的輸入、操作和預期輸出。

### 2. 選擇測試工具與環境

- 根據 `test_requirements` 和 `system_under_test_info`，選擇合適的測試工具和環境。
- 如果提供了 `testing_framework_preference`，則優先使用。

### 3. 設計測試用例

- 為每個測試場景設計詳細的測試用例，包括前置條件、測試步驟、測試數據和預期結果。
- 考慮邊界條件和異常情況。

### 4. 編寫測試腳本

- 使用選定的測試框架和語言編寫自動化測試腳本。
- 確保腳本的可讀性、可維護性和可重用性。
- 包含必要的斷言 (assertions) 來驗證結果。

### 5. 執行與調試

- 在測試環境中執行測試腳本。
- 根據執行結果進行調試，修正腳本中的錯誤。

### 6. 報告測試結果

- 生成測試執行報告，包括通過、失敗的測試用例和錯誤訊息。

## Outputs

- **`test_script_code`**: 開發完成的測試腳本程式碼。
- **`test_execution_report`**: 測試腳本的執行結果報告。
- **`test_cases_document`** (Optional): 詳細的測試用例文檔。

## Key Principles

- **自動化**: 盡可能實現測試過程的自動化。
- **可重複性**: 測試腳本應能在不同環境下重複執行並得到一致結果。
- **精準性**: 測試腳本應能準確驗證功能，並捕獲錯誤。
- **可維護性**: 腳本應易於理解和修改。
