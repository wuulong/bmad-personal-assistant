<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 生成測驗題 (Create Quiz)

## Purpose

此任務旨在根據使用者提供的學習內容，生成一份測驗題，幫助使用者檢測學習成果，鞏固知識。

## Inputs

- **`learning_content`**: 用於生成測驗題的學習內容（文字、URL 或文件路徑）。
- **`quiz_type`** (Optional): 測驗題類型（例如：選擇題、判斷題、簡答題）。
- **`num_questions`** (Optional): 期望的題目數量。
- **`difficulty_level`** (Optional): 測驗題的難度（例如：簡單、中等、困難）。

## Process

### 1. 接收與解析內容

- 接收 `learning_content`，並根據其類型進行解析。
- 確保內容的完整性和可讀性，以便提取考點。

### 2. 識別考點與知識點

- 分析學習內容，識別其中重要的概念、定義、事實、流程和應用場景。
- 根據 `difficulty_level` 調整考點的深度和廣度。

### 3. 生成測驗題目

- 根據識別出的考點和 `quiz_type`，生成具體的測驗題目。
- 對於選擇題，生成正確答案和合理的干擾項。
- 對於判斷題，確保陳述的準確性。
- 對於簡答題，明確問題的核心要求。

### 4. 提供答案與解析

- 為每道題目提供正確答案。
- 對於需要解釋的題目，提供簡潔明瞭的解析。

## Outputs

- **`quiz_questions`**: 生成的測驗題目清單。
- **`quiz_answers`**: 測驗題目的答案。
- **`quiz_explanations`** (Optional): 測驗題目的解析。

## Key Principles

- **針對性**: 題目應緊密圍繞學習內容的核心知識點。
- **多樣性**: 盡可能涵蓋不同類型的題目，以全面檢測。
- **清晰性**: 題目表述應清晰無歧義。
- **有效性**: 題目應能有效評估學習者的理解程度。
