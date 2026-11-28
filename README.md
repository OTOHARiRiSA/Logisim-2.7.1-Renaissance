# Logisim Renaissance

Logisim Renaissance 延續 Carl Burch 開發的原版 Logisim，讓它更容易在現代作業系統上建置與執行，同時保留原有的功能與使用方式。

Logisim Renaissance maintains Carl Burch’s original Logisim for modern operating systems while preserving its original features and behavior.

本專案保留了從 SourceForge SVN 遷移而來的提交歷史。Carl Burch 最後正式發布的版本是 2.7.1，Renaissance 的 2.7.2 則源自原始 SVN 倉庫中尚未發布的開發版本。

This repository preserves the commit history migrated from SourceForge SVN. Carl Burch’s last official release was 2.7.1. Renaissance 2.7.2 was based on an unreleased development snapshot from the original SVN repository.

## 下載與安裝 / Download and install

[下載最新正式版 / Download the latest release](https://github.com/OTOHARiRiSA/Logisim-Renaissance/releases/latest)

請在發行頁面的 **Assets** 選擇適合的平台與格式。Windows 與 macOS 套件已內建 Java 執行環境。使用獨立 JAR 時，請自行安裝 Java，建議使用 Java 25。

Choose the appropriate download under **Assets** on the release page. The Windows and macOS packages bundle a Java runtime. To run the standalone JAR, install Java separately. Java 25 is recommended.

| 平台 / Platform | 格式 / Format | 使用方式 / How to use |
| --- | --- | --- |
| Windows x86-64 | EXE 或 MSI | 執行安裝程式。 / Run the installer. |
| Windows x86-64 | ZIP | 解壓縮後執行資料夾中的 Logisim Renaissance。 / Extract the archive and launch Logisim Renaissance from the extracted folder. |
| macOS Apple Silicon | DMG | 開啟磁碟映像，將應用程式拖入「應用程式」資料夾。 / Open the disk image and drag the app into Applications. |
| 其他可執行 Java 的平台 / Other platforms with Java | JAR | 使用 `java -jar` 執行下載的 JAR。 / Run the downloaded JAR with `java -jar`. |

未簽署或未經公證的套件可能觸發 Windows SmartScreen 或 macOS Gatekeeper 提示。請從本專案的 GitHub Releases 下載。

Unsigned or unnotarized packages may trigger Windows SmartScreen or macOS Gatekeeper prompts. Download packages from this project’s GitHub Releases page.

## 本地化與建置 / Localization and builds

2.8.0 的開發加入了簡體中文介面，並將多語系資源遷移至 UTF-8。GitHub Actions 在 Windows、macOS 和 Linux 上建置 JAR，並使用 Eclipse Temurin 25 提供的 `jpackage` 建立 Windows 與 macOS 套件。

Development for 2.8.0 added a Simplified Chinese interface and migrated localization resources to UTF-8. GitHub Actions builds the JAR on Windows, macOS, and Linux, and uses `jpackage` from Eclipse Temurin 25 to build the Windows and macOS packages.

## 貢獻 / Contributing

歡迎協助測試、修正問題、改善文件或參與翻譯。本機建置與貢獻方式請參閱 [CONTRIBUTING.md](CONTRIBUTING.md)。

Testing, bug fixes, documentation improvements, and translations are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for local build instructions and ways to contribute.

## 授權 / License

- Carl Burch 開發的原版 [Logisim](https://www.cburch.com/logisim/) 採用 GNU GPL v2 或更新版本。 / Carl Burch’s original Logisim is licensed under GNU GPL v2 or later.
- Windows 與 macOS 套件內建的 [Eclipse Temurin](https://adoptium.net/) 採用 GPL v2 with the Classpath Exception。 / The Eclipse Temurin runtime bundled with the Windows and macOS packages is licensed under GPL v2 with the Classpath Exception.
- 本專案的授權條款詳見 [LICENSE](LICENSE)。 / See [LICENSE](LICENSE) for the project’s license terms.
