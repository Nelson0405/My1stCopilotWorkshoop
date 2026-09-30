# 待辦清單 Web App

這是一個在 GitHub Copilot 實戰工作坊中逐步完成的純前端待辦清單應用程式，涵蓋需求描述、多檔修改、瀏覽器驗證與 Git 版本管理。

## 線上展示

預計網址：[https://nelson0405.github.io/My1stCopilotWorkshoop/](https://nelson0405.github.io/My1stCopilotWorkshoop/)

GitHub Pages 已從 `main` 分支的根目錄部署，網站已可公開瀏覽。

## 功能

- 新增待辦，空白內容不會送出。
- 標記完成或取消完成，並可刪除單筆待辦。
- 顯示整體未完成項目數量。
- 依全部、未完成、已完成篩選待辦。
- 切換深色與淺色模式；記住手動選擇，初次使用時跟隨作業系統偏好。
- 將待辦資料與主題偏好保存在瀏覽器 `localStorage`。
- 支援手機版面與鍵盤操作。

## 技術

- HTML、CSS 與原生 JavaScript。
- 不使用框架、套件或外部 CDN，可離線開啟。
- CSS 以自訂屬性管理淺色與深色主題。
- 使用瀏覽器 `localStorage` 保存待辦資料與主題偏好。

## 開發方式

- 使用 GitHub Copilot Agent Mode 依需求跨檔案實作功能，並在瀏覽器驗證互動。
- 在 `.vscode/mcp.json` 設定 Microsoft Learn 與 GitHub MCP Server；伺服器需在 VS Code 中啟動及授權，本專案尚未確認其執行狀態。
- 建立 `.github/copilot-instructions.md` 作為專案規範，並以 `.github/prompts/fix-issue.prompt.md` 描述 issue 修復流程及人工確認步驟。
- Issue #3 的修正已推送至 `fix/issue-3`，但尚未建立或合併 Pull Request。

## 我學到什麼

- 把需求與限制寫清楚，有助於 Agent 一次處理多個相關檔案。
- 修改完成後要用實際操作驗證，而不只看程式碼差異。
- Git 分支與提交能讓功能修改和主線分開管理。
- MCP 需要設定並在用戶端啟動，才能讓 Agent 使用外部服務。
- 將重複流程寫成 prompt，並保留人工確認點，能讓協作步驟更一致。