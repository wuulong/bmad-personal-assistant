<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 清理數據 (Clean Data)

## Purpose

此任務旨在識別並建議修正數據中的不一致或錯誤，以提高數據品質，確保數據的準確性和可靠性。

## Inputs

- **`raw_data`**: 需要清理的原始數據集。
- **`data_schema`** (Optional): 數據的預期結構或模式定義。
- **`cleaning_rules`** (Optional): 特定的數據清理規則或標準。

## Process

### 1. 數據審查與問題識別

- 仔細審查 `raw_data`，識別潛在的數據品質問題，例如：
    - 缺失值 (Missing values)
    - 異常值 (Outliers)
    - 重複記錄 (Duplicate records)
    - 格式不一致 (Inconsistent formats)
    - 數據類型錯誤 (Incorrect data types)
    - 邏輯錯誤 (Logical errors)
- 參考 `data_schema` 和 `cleaning_rules` 進行問題判斷。

### 2. 建議清理策略

- 針對識別出的每個問題，建議合適的清理策略或修正方法。
- 例如：
    - 填充缺失值（平均值、中位數、眾數或模型預測）。
    - 移除或轉換異常值。
    - 刪除重複記錄。
    - 統一數據格式（日期、文字大小寫、單位）。
    - 修正數據類型。

### 3. 執行數據清理（或提供清理指令）

- 如果可能，直接執行數據清理操作。
- 如果需要使用者確認或手動干預，則提供詳細的清理指令和建議。

### 4. 驗證清理結果

- 檢查清理後的數據，確保問題已得到解決，且沒有引入新的錯誤。
- 評估數據品質的提升程度。

## Outputs

- **`cleaned_data`**: 清理後的數據集。
- **`cleaning_report`**: 數據清理過程的報告，包括識別出的問題、採用的策略和清理前後的數據品質對比。
- **`suggested_corrections`** (Optional): 如果無法自動清理，提供給使用者的修正建議。

## Key Principles

- **準確性**: 確保清理後的數據真實反映現實。
- **一致性**: 數據在格式和內容上應保持一致。
- **完整性**: 盡可能保留數據的完整性，避免不必要的數據丟失。
- **可追溯性**: 清理過程應有記錄，方便回溯和審查。
