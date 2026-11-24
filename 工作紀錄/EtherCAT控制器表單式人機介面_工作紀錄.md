# EtherCAT 控制器表單式人機介面｜專案工作紀錄

> 依 WITS 專案履歷表整理，功能涵蓋虛擬化資料表格、控制器即時通訊及雲端 FTP 更新。

## 基本資料
- 公司：動程科技股份有限公司
- 專案期間：2016/01–2019/09
- 專案角色：SD；職掌為軟體開發（依專案履歷表原文）
- 開發工具：Visual Studio Code
- 前端：ReactJS、Redux、React Virtualized、Material UI
- 後端：Node.js、Express
- 來源：WITS_專案履歷表__周蔓君.doc、cv/Interview.md、cv/2026.md

## 專案概述與本人工作
開發用於 EtherCAT 控制器管理的表單式即時控制介面。專案履歷表記載的工作包括：
- 開發大量資料渲染的虛擬滾動介面，使用 React Virtualized。
- 使用 WebSocket 與控制器進行即時通訊。
- 實作表格即時更新與操作回寫。
- 建立雲端 FTP 更新機制。

## 技術與功能紀錄
- **前端：**ReactJS、Redux、React Virtualized、Material UI。
- **後端：**Node.js、Express。
- **即時通訊：**WebSocket。
- **介面功能：**表格式動態顯示及控制操作、資料即時更新與回寫。
- **更新功能：**雲端 FTP 下載更新。

## 結果與證據
- 已記載交付：控制器即時操作介面、虛擬化資料呈現、WebSocket 通訊及 FTP 更新功能。
- 控制器數量、資料列規模、更新頻率、實際上線情況及效益數據：待補。
- 證據：待補可安全引用的程式碼審查、測試或發布紀錄。

## 履歷摘要草稿
開發 EtherCAT 控制器表單式即時操作介面，使用 React Virtualized 呈現大量資料，透過 WebSocket 與控制器即時通訊，並實作表格更新回寫及雲端 FTP 更新。

## 待本人確認
- [ ] React Virtualized 的資料規模與虛擬化方式。
- [ ] WebSocket 訊息格式、斷線處理及資料一致性策略。
- [ ] 操作回寫及控制器回應的驗證流程。
- [ ] FTP 更新的觸發條件、版本管理及失敗回復方式。
