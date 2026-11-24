# Inline Config Manager｜專案工作紀錄

> 依 WITS 專案履歷表補入期間、工作範圍與技術；功能細節另參考 tmp/InlineConfigManager.md。個人工作項目依專案履歷表記載，成果數據與上線成效未提供。

## 基本資料
- 專案公司／客戶：台積電
- 雇主：緯創軟體股份有限公司（依個人履歷任職資料）
- 專案期間：2025/10–2026/04
- 專案角色：SD；職掌為軟體開發（依專案履歷表原文）
- 開發工具：Visual Studio Code
- 技術：React Hooks、Redux Toolkit、React Router、AgGrid
- 來源：WITS_專案履歷表__周蔓君.doc、tmp/InlineConfigManager.md

## 專案概述
維護及新增使用者需求，開發讓使用者自行操作機台相關設定變更的系統。功能涵蓋 Inline Config Manager 的多個設定頁面，包括 Lot Forecast、Fanout、Rollback、Litho Defense、CDSEM Tool Management、Event List、IDP Config Setting、Delay Dock 及 Mediator Rule。

## 本人負責工作
專案履歷表記載本人負責維護及新增使用者需求，並開發使用者可自行操作機台設定變更的系統。核心職責包括：
- 建立對應 Tool 的 Event List 表單。
- 提供表單欄位 popup，以顯示擴充資料。
- 建立設定資料編輯頁面。
- 提供表格資料新增、刪除、修改功能。
- 提供 CSV 批次修改功能。

## 功能與流程紀錄
### Lot Forecast 編輯
- 新增／修改編輯頁面，包含三個分頁，支援逐筆編輯、新增及刪除。
- 支援批次上傳並取代原表單；上傳後暫不更新，送出時先顯示影響清單及警告，確認後才送出。
- 預測模型尚未定義時，可由 Fanout 跨廠帶入資料。

### Rollback
- 依資料類型 Fanout 或 Edit 導向不同的 rollback 頁面。

### Litho Defense、CDSEM、Delay Dock
- Litho Defense 支援使用者上傳 rule 與 alarm action；其 Event List 需填入文字型 unitName。
- CDSEM Tool Management 從僅能新增擴充為可修改及刪除既有項目；另可更新亂數選點設定與機台 IP。
- Delay Dock 用於驗證 mediator rule 設定是否缺漏。

### Event List 與 Mediator Rule
- Fab 選定後篩選 EPT ToolType，ToolType 單選並提供 ALL 選項。
- ToolType 未選 ALL 時，ID 選項過濾並加入 ALL；選取 ALL 時，ID 不再顯示 ALL；最多 20 筆。
- Mediator Rule 總表沒有系統入口，透過 URL 連結進入。

## 結果與證據
- 已記載交付：Event List、設定資料編輯、表格 CRUD、CSV 批次修改及多類設定維護頁面。
- 使用量、設定變更處理時間、錯誤率或上線成效：來源未提供，待補可驗證資料。
- 證據：待補可安全引用的需求單、PR、驗收或發布紀錄。

## 技術與設計細節待補
- 各頁面的本人實作範圍、與團隊成員的分工。
- CSV 格式、欄位驗證、錯誤回饋及批次更新失敗處理。
- 批次上傳影響清單的資料來源、計算方式與防錯設計。
- 實際測試及驗收流程。

## 履歷摘要草稿
維護並新增 Inline Config Manager 使用者需求，開發機台設定變更平台，建立 Tool 對應 Event List、設定資料編輯與表格 CRUD，並提供 CSV 批次修改功能。

## 待本人確認
- [ ] 專案中各子系統頁面的實際負責範圍。
- [ ] 台積電為專案客戶／使用單位；雇主及駐點資訊是否需在正式履歷標明。
- [ ] 批次修改的實際使用規模與可驗證成效。
