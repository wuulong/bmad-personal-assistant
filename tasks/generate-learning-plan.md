<!-- Powered by BMAD™ Personal Assistant Expansion Pack -->

# 生成學習計畫 (Generate Learning Plan)

## Purpose

此任務旨在根據使用者提供的學習目標和時間，生成一份詳細、個性化的學習計畫，幫助使用者高效達成學習目標。

## Inputs

- **`learning_goal`**: 使用者明確的學習目標（例如：掌握 Python 基礎、通過某項考試、學習新技能）。
- **`available_time`**: 使用者每天或每週可投入學習的時間。
- **`current_knowledge_level`** (Optional): 使用者目前對該領域的知識水平。
- **`preferred_learning_style`** (Optional): 使用者偏好的學習方式（例如：閱讀、影片、實作、聽講）。

## Process

### 1. 理解學習目標與約束

- 深入分析 `learning_goal`，將其分解為可衡量的子目標。
- 考慮 `available_time` 作為計畫的硬性約束。
- 評估 `current_knowledge_level`，確定學習起點。

### 2. 規劃學習路徑

- 根據學習目標和時間，設計合理的學習階段和里程碑。
- 建議學習內容的順序和重點。
- 考慮不同學習資源的整合（例如：書籍、線上課程、實作專案）。

### 3. 建議學習方法與資源

- 根據 `preferred_learning_style`，推薦適合的學習方法和具體資源。
- 提供高效學習技巧（例如：費曼技巧、間隔重複）。

### 4. 制定時間表與進度追蹤

- 為每個學習階段或子目標分配具體時間。
- 建議進度追蹤方式和評估方法。
- 預留彈性時間以應對突發情況。

## Outputs

- **`learning_plan_document`**: 一份詳細的學習計畫，包含：
    - 學習目標分解。
    - 學習內容大綱。
    - 推薦學習資源。
    - 時間表與進度安排。
    - 學習方法建議。

## Key Principles

- **個性化**: 根據使用者具體情況量身定制。
- **可行性**: 計畫應切合實際，避免過度承諾。
- **階段性**: 將大目標分解為小階段，易於執行和追蹤。
- **彈性**: 允許根據學習進度或外部變化進行調整。
