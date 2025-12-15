# 個人簡歷網站與 Git 實作驗收

---
## Git 版本控制與 A/B Test 驗收說明

### 1. 版本回復 (Git Revert) 練習

我在這次作業中使用 `git revert` 回復了 Commit `3ef7b29` (feat: complete personal content and add profile photo)。

**回復原因：** 這是作業中的版本控制練習要求。我們在開發 `feature/skills-tags` 分支 (版本 B) 後，需要證明能夠將 `main` 分支回溯到 A/B Test 開始之前的狀態 (版本 A)，以確保測試流程的穩定性。

### 2. A/B Test 決策說明

| 版本 | 分支 | 狀態 | 說明 |
| :--- | :--- | :--- | :--- |
| **版本 A (進度條)** | N/A | **未採用** | 提供了清晰的技能熟練度百分比。 |
| **版本 B (標籤雲)** | `feature/skills-tags` | **採用** | 視覺效果更美觀，且成功應用了 CSS 標籤雲和響應式設計，更符合個人簡歷的設計趨勢。 |

**最終決定：** 採用 **版本 B (標籤雲)** 作為最終部署版本，已將 `feature/skills-tags` 的 PR 合併回 `main`。