# Logisim Renaissance 2.7.x

這是基於 Carl Burch 原版 Logisim 的維護與重新打包專案，主要是為了讓舊版 Logisim 在現代作業系統上更容易建置和執行，並盡可能保留原有的功能與使用方式。

This project maintains and repackages Carl Burch's original Logisim to make it easier to build and run on modern operating systems, while preserving its original functionality and behavior as much as possible.

目前使用的 2.7.2 程式碼來自原始 SVN 倉庫中尚未正式發布的開發版本。Carl Burch 最後正式發布的版本是 2.7.1。

Version 2.7.2 is based on unreleased development code from the original SVN repository. The last official release by Carl Burch was 2.7.1.

## 下載與安裝 / Download and install

[下載 Logisim Renaissance / Release downloads](https://github.com/OTOHARiRiSA/Logisim-2.7.x-Renaissance/releases)

目前提供 Windows x86-64 版本，內建 Java 執行環境，無需另外安裝 Java。

Windows x86-64 packages are currently available. They include a Java runtime, so no separate Java installation is required.

| 格式 / Format | 安裝方式 / Installation |
| --- | --- |
| ZIP | 解壓縮後執行 `Logisim-Renaissance.exe`，無需安裝。 / Extract the archive and run `Logisim-Renaissance.exe`. |
| EXE | 執行安裝程式，依照畫面指示安裝。 / Run the installer and follow the instructions. |
| MSI | 使用 Windows Installer 安裝。 / Install using Windows Installer. |

macOS 和 Linux 的發行包尚未提供。

macOS and Linux packages are not yet available.

## 這是如何做的？ / How was this built?

本專案保留了原版 Logisim 的 Java 原始碼，以及從 SourceForge SVN 遷移而來的提交歷史。

The repository preserves the original Logisim Java source code and commit history migrated from SourceForge SVN.

目前僅對原始碼與建置流程進行少量相容性修改，包括移除一處 UTF-8 BOM，以及更新舊版 Java 編譯參數。

Only minor compatibility changes have been made to the source and build process, including removing a UTF-8 BOM and updating the Java compiler options.

Windows 發行包使用 **Eclipse Temurin 25 (OpenJDK)** 提供的 `jpackage` 建立，並內建 Java 執行環境。

The Windows packages are built using `jpackage` from **Eclipse Temurin 25 (OpenJDK)** and include a bundled Java runtime.

## 授權 / License

- **Logisim** 由 Carl Burch 開發，原始碼依 GNU GPL v2 或更新版本授權。 / Logisim was developed by Carl Burch and is licensed under GPL v2 or later. [Logisim](https://www.cburch.com/logisim/)
- **Eclipse Temurin (OpenJDK)** 使用 GPL v2 with Classpath Exception。Windows 發行包內建 Temurin 25 執行環境。 / The Windows packages bundle an Eclipse Temurin 25 runtime, licensed under GPL v2 with the Classpath Exception. [Eclipse Temurin](https://adoptium.net/)
- **Logisim Renaissance** 的授權條款詳見 [LICENSE](LICENSE)。 / See [LICENSE](LICENSE) for the applicable license terms.
