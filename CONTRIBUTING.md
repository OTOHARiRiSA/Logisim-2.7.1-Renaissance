# Contributing to Logisim Renaissance
# Logisim Renaissance 貢獻指南

Thank you for your interest in contributing to **Logisim Renaissance**!

Logisim Renaissance is an independent community effort to maintain, develop, and distribute Carl Burch's original Logisim for modern systems.

Whether you are an experienced developer or simply someone who enjoys exploring old software, you are welcome to participate.

感謝你有興趣參與 **Logisim Renaissance**！

Logisim Renaissance 是一個獨立的社群項目，致力於維護、開發與發行 Carl Burch 的原版 Logisim，使其能夠在現代系統上繼續使用。

無論你是經驗豐富的開發者，還是單純喜歡研究老軟件的人，都歡迎一起參與。

**Our philosophy is simple: Just for fun.**

**我們的理念很簡單：Just for fun。**

---

## 1. Before You Start / 開始之前

### 1.1 Prerequisites / 前置要求

All maintainers and contributors **MUST** watch the following video:

所有 Maintainer 和 Contributors **必須**觀看以下影片：

https://www.bilibili.com/video/BV1pwC6BxEeb

This video is a joke. Understanding why it is a joke is not optional.

這個影片是個玩笑，但理解它為什麼是個玩笑不是可選項。

### 1.2 You Don't Need to Be an Expert / 不必成為專家

You do not need extensive programming experience to contribute.

Contributions may include:

- Bug reports and testing
- Documentation improvements
- Translations and localization
- Build and packaging improvements
- Compatibility fixes
- New features and enhancements

你不需要具備豐富的編程經驗才能參與。

貢獻可以包括：

- 回報 Bug 與協助測試
- 改善文檔
- 翻譯與本地化
- 改進構建及打包流程
- 修復兼容性問題
- 新功能與功能改進

Please be willing to learn, communicate, and take responsibility for your contributions.

請保持學習與交流的意願，並對自己的貢獻負責。

---

## 2. Understanding the Project / 了解項目

Logisim Renaissance is based on the original Logisim source code developed by Carl Burch.

The last official release by Carl Burch was **2.7.1**. Version **2.7.2** in this project is based on unreleased development code from the original SVN repository.

Logisim Renaissance is independently maintained and is not an official release by Carl Burch.

Logisim Renaissance 基於 Carl Burch 開發的原版 Logisim 源碼。

Carl Burch 最後正式發布的版本是 **2.7.1**。本項目的 **2.7.2** 基於原始 SVN 倉庫中尚未正式發布的開發代碼。

Logisim Renaissance 由社群獨立維護，並非 Carl Burch 的官方發行版本。

### 2.1 Development Environment / 開發環境

Logisim Renaissance supports both automated and manually configured development environments.

The use of mise-en-place is recommended but not mandatory.

Logisim Renaissance 同時支持自動配置及手動配置的開發環境。

我們推薦使用 mise-en-place，但並不強制要求。

#### With mise-en-place / 使用 mise-en-place

Install mise-en-place by following its official documentation:

從官方網站下載 mise-en-place：

https://mise.jdx.dev/

After cloning the repository, run the following commands from the repository root:

完成倉庫 Clone 後，在倉庫根目錄執行以下命令：

```sh
mise trust
mise install
```

The required toolchain versions are declared in `mise.toml`.

所需的工具鏈版本已在 `mise.toml` 中聲明。

#### Without mise-en-place / 不使用 mise-en-place

Contributors may configure their development environments manually by installing the tools declared in `mise.toml`.

貢獻者也可以自行安裝 `mise.toml` 中聲明的工具，以手動配置開發環境。

The primary development tools include:

主要開發工具包括：

- Git
- Java Development Kit (JDK 25, Eclipse Temurin recommended)
- Python 3.12

Ensure that the required executables are available in your `PATH`, and configure `JAVA_HOME` where necessary.

請確保所需的可執行文件已加入 `PATH`，並在需要時配置 `JAVA_HOME`。

### 2.2 Editors and IDEs / 編輯器與 IDE

Contributors are free to choose their preferred editors and IDEs. No specific editor or IDE is required.

貢獻者可以自由選擇自己喜歡的編輯器或 IDE，本項目不強制要求使用任何特定的開發工具。

### 2.3 Documentation and Translation / 文檔與翻譯

Contributors working exclusively on documentation or translations are not required to configure the complete build toolchain before making contributions.

僅參與文檔或翻譯工作的貢獻者，不需要在開始貢獻前配置完整的構建工具鏈。

Please save all text files using UTF-8 encoding and preserve the existing document structure.

請使用 UTF-8 編碼保存所有文本文件，並保留既有的文檔結構。

### 2.4 Our Goals / 項目目標

- Preserve the original Logisim's functionality and behavior.
- Keep the software buildable and usable on modern systems.
- Improve maintenance, development, and distribution.
- Welcome community contributions while respecting the project's history.

我們希望：

- 保留原版 Logisim 的功能與行為。
- 使其能在現代系統上持續構建與運行。
- 改進維護、開發及發行流程。
- 在尊重項目歷史的前提下，歡迎社群參與。

**Legacy behavior should remain the default. Experimental behavior should be opt-in.**

**既有行為應當保持默認，實驗性行為應由使用者主動啟用。**

---

## 3. Downloading and Testing / 下載與測試

### 3.1 Releases Are Not Source Code / 發行包不是源碼

If you only want to use or test Logisim Renaissance, **you do not need to download or compile the source code**.

Visit the Releases page:

https://github.com/otoharirisa/Logisim-2.7.x-Renaissance/releases

Select a release and download the appropriate file from its **Assets** section.

如果你只是想使用或測試 Logisim Renaissance，**不需要下載或編譯源碼**。

請前往 Releases 頁面：

https://github.com/otoharirisa/Logisim-2.7.x-Renaissance/releases

選擇一個發行版本，然後從 **Assets** 區域下載對應文件。

### 3.2 Windows Packages / Windows 發行包

| Package / 文件 | Purpose / 用途 |
|---|---|
| ZIP | Portable distribution / 便攜版，解壓後運行 |
| Setup.exe | Windows installer / Windows 安裝程序 |
| MSI | Windows Installer package / Windows Installer 安裝包 |
| Source code | For development / 供開發者使用的源碼 |

**Important:** The automatically generated `Source code (zip)` and `Source code (tar.gz)` archives on GitHub are not prebuilt applications.

**注意：** GitHub 自動生成的 `Source code (zip)` 和 `Source code (tar.gz)` 是源碼壓縮包，不是已構建好的應用程序。

### 3.3 What to Test / 測試內容

When testing a release, please check:

1. Whether the package can be downloaded.
2. Whether installation or extraction succeeds.
3. Whether Logisim starts correctly.
4. Whether existing `.circ` files can be opened.
5. Whether basic circuit editing and simulation work.
6. Whether the installed application can be uninstalled correctly, where applicable.

測試發行包時，請確認：

1. 能否正常下載文件。
2. 能否正常安裝或解壓。
3. Logisim 能否正常啟動。
4. 能否打開既有的 `.circ` 文件。
5. 基本電路編輯與模擬功能是否正常。
6. 對於安裝版，能否正常卸載。

If Windows or your browser displays a security warning, please report the exact message. Do not disable system-wide security protection just to complete a test.

如果 Windows 或瀏覽器顯示安全警告，請回報具體內容。不要為了完成測試而關閉整個系統的安全防護。

---

## 4. Reporting Issues / 回報問題

Before opening a new Issue, please check whether a similar issue already exists.

When reporting a bug, include:

- Operating system and version
- Logisim Renaissance version
- Package type, if applicable
- Steps to reproduce the problem
- Expected behavior
- Actual behavior
- Relevant logs or screenshots

建立新 Issue 前，請先確認是否已有相同或類似的問題。

回報 Bug 時，請盡量提供：

- 操作系統及版本
- Logisim Renaissance 版本
- 使用的發行包類型（如適用）
- 問題重現步驟
- 預期行為
- 實際行為
- 相關日誌或截圖

Please describe the problem clearly and avoid reporting unrelated problems in a single Issue.

請清楚描述問題，並盡量避免將多個無關問題放在同一個 Issue 中。

---

## 5. Contributing Code / 代碼貢獻

### 5.1 Basic Workflow / 基本流程

1. Fork the repository.
2. Clone your fork to your local machine.
3. Create a branch for your changes.
4. Make and test your changes.
5. Commit your changes with a meaningful message(Conventional Commits).
6. Push the branch to your fork.
7. Open a Pull Request against the upstream repository.

基本流程如下：

1. Fork 本倉庫。
2. 將 Fork 後的倉庫 Clone 到本地。
3. 為修改建立獨立分支。
4. 完成修改並進行測試。
5. 使用有意義的 Commit Message （Conventional Commits）提交修改。
6. 將分支 Push 到自己的倉庫。
7. 向上游倉庫提交 Pull Request。

Example / 示例：

```bash
git clone https://github.com/YOUR_USERNAME/Logisim-2.7.x-Renaissance.git
cd Logisim-2.7.x-Renaissance

git switch -c fix/example-issue

# Make your changes
# 進行修改

git add .
git commit -m "fix: describe the change"
git push -u origin fix/example-issue
```

Replace `YOUR_USERNAME` with your GitHub username.

請將 `YOUR_USERNAME` 替換為你的 GitHub 使用者名稱。

If you are unfamiliar with Git or Pull Requests, feel free to ask questions before submitting changes.

如果你還不熟悉 Git 或 Pull Request，歡迎先提出問題。

### 5.2 Pull Request Guidelines / PR 規範

Please:

- Keep each PR focused on a clear purpose.
- Explain what you changed and why.
- Describe how you tested the changes.
- Avoid unrelated formatting or refactoring changes.
- Discuss major architectural changes before implementation.
- Be prepared to respond to review feedback.

請盡量：

- 讓每個 PR 專注於明確的目標。
- 說明修改內容及原因。
- 描述測試方式與結果。
- 避免無關的格式化或重構。
- 在進行重大架構修改前先討論。
- 願意根據 Review 意見調整修改。

A PR does not need to be perfect when first opened. Discussion and iteration are part of open-source development.

PR 不必在第一次提交時就完美。討論與反覆修改本來就是開源開發的一部分。

---

## 6. Compatibility and Coding Principles / 兼容性與編程原則

Logisim Renaissance is a continuation of a legacy software project.

Please respect the existing architecture and behavior.

In particular:

- Preserve compatibility with existing `.circ` files whenever possible.
- Avoid unintended changes to circuit simulation semantics.
- Do not introduce breaking changes without prior discussion.
- Prefer small, understandable changes over unnecessary rewrites.
- Keep experimental behavior optional where practical.
- Avoid introducing dependencies without a clear reason.

Logisim Renaissance 是一個延續既有軟件生命週期的項目。

請尊重原有架構及行為。

尤其需要注意：

- 盡可能維持與既有 `.circ` 文件的兼容性。
- 避免意外改變電路模擬語義。
- 未經討論，不要引入破壞性變更。
- 優先採用小而清晰的修改，避免不必要的重寫。
- 在可行的情況下，讓實驗性行為保持可選。
- 不要在缺乏明確理由的情況下增加依賴。

Modernization is welcome, but modernization alone is not a reason to break existing behavior.

我們歡迎現代化改進，但「現代化」本身不是破壞既有行為的理由。

---

## 7. Localization and Translation / 本地化與翻譯

Translations are welcome, including Simplified Chinese, Traditional Chinese, and other languages.

Please:

- Follow the project's existing localization mechanism.
- Preserve resource keys and placeholders.
- Keep technical terminology consistent.
- Test translated text in the application.
- Avoid unrelated changes to program logic.
- Respect the licensing and attribution requirements of any external translation material.

我們歡迎翻譯貢獻，包括簡體中文、繁體中文及其他語言。

請注意：

- 遵循項目既有的本地化機制。
- 保留資源鍵名及佔位符。
- 保持技術術語一致。
- 在程序中實際檢查翻譯效果。
- 避免同時修改無關的程序邏輯。
- 使用其他翻譯資料時，尊重其授權及署名要求。

Existing translations may be useful references, but they should not be copied into the project without checking their origin and licensing.

既有漢化版本可以作為參考，但在確認來源及授權之前，不應直接將其內容複製進本項目。

You are welcome to start with a small translation PR instead of translating the entire application at once.

歡迎先從小範圍的翻譯 PR 開始，不必一次完成整個程序的漢化。

---

## 8. AI-Assisted Contributions / AI 輔助貢獻

AI tools may be used to assist with development, documentation, translation, and debugging.

However, contributors are responsible for everything they submit.

Please ensure that:

- You understand the changes you submit.
- AI-generated code has been reviewed and tested.
- You can explain how your changes work.
- Generated content does not introduce licensing or security problems.
- You do not submit large amounts of unreviewed AI-generated code.

可以使用 AI 工具輔助開發、文檔編寫、翻譯及調試。

但貢獻者必須對自己提交的所有內容負責。

請確保：

- 理解自己提交的修改。
- 已審查並測試 AI 生成的代碼。
- 能夠解釋修改的工作原理。
- 生成內容不會引入授權或安全問題。
- 不提交大量未經審查的 AI 生成代碼。

**AI assistance is welcome. Blindly submitting generated code is not.**

**我們歡迎 AI 輔助，但不歡迎不經理解與審查就提交生成代碼。**

---

## 9. Review and Maintenance / 審查與維護

All contributions may be reviewed before merging.

Maintainers may request changes, suggest alternatives, or decline contributions that conflict with the project's goals.

Review is intended to improve the project, not to discourage contributors.

所有貢獻在合併前都可能需要經過 Review。

Maintainer 可以要求修改、提出替代方案，或拒絕與項目目標不符的貢獻。

Review 的目的是改善項目，而不是打擊貢獻者的積極性。

Please communicate respectfully and focus discussions on technical issues and project goals.

請尊重其他參與者，並盡量讓討論聚焦於技術問題和項目目標。

---

## 10. Just for Fun / 只是為了好玩

Logisim Renaissance is a hobby-driven open-source project.

There are no contribution quotas, mandatory schedules, or expectations that everyone must be available all the time.

You are welcome to explore, learn, experiment, and contribute at your own pace.

Logisim Renaissance 是一個由興趣驅動的開源項目。

這裡沒有貢獻數量指標、強制開發進度，也不要求每個人隨時在線。

歡迎按照自己的節奏探索、學習、實驗和貢獻。

We value curiosity, understanding, collaboration, and respect for the original software.

我們重視好奇心、理解、協作，以及對原始軟件的尊重。

**Have fun, and happy hacking!**

**玩得開心，Happy Hacking！**
