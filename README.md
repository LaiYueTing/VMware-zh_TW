# [VMware Workstation 繁體中文化][project-url]

  [![GitHub issues][issues-image]][issues-url]
  [![GitHub stars][stars-image]][stars-url]
  [![GitHub forks][forks-image]][forks-url]
  [![license GPL-3.0][license-image]][license-url]

為 VMware Workstation Pro 提供台灣繁體中文 (`zh_TW`) 介面語言檔。

> [!NOTE]
>
> 自新版本命名規則 (`25H2`) 起，Broadcom 已從安裝套件中移除包含中文在內的部分多國語言。
> 本專案提供的語言檔可放回安裝目錄，讓新版本重新顯示繁體中文介面。

## 📝 目前版本

| 項目 | 版本 |
| --- | --- |
| 主程式版本 | VMware Workstation Pro 26H1u1 Build 25688693 |
| 語言檔版本 | 26.0.1.2799 |

### 版本對照表

本儲存庫只保留最新版本的語言檔，歷史版本可從對應的 [標籤 (Tag)][tags-url] 下載。

| 語言檔版本 | 對應主程式版本 | 標籤 |
| --- | --- | --- |
| 26.0.1.2799 | 26H1u1 Build 25688693 | `v26.0.1.2799` |
| 17.6.0.61175 | 17.6.0 Build 24238078 | `v17.6.0.61175` |
| 17.5.2.59081 | 17.5.2 Build 23775571 | `v17.5.2.59081` |
| 17.5.1.55451 | 17.5.1 Build 23298084 | `v17.5.1.55451` |

> [!WARNING]
>
> 語言檔須與主程式版本相符。版本不符時，新增的功能或介面可能缺少翻譯，或顯示異常。

## 📦 檔案說明

```text
zh_TW/
├── vmappsdk-zh_TW.dll   # 應用程式資源 (對話方塊、選單、字串表)
├── vmui-zh_TW.dll       # 使用者介面資源 (對話方塊、選單)
└── vmware.vmsg          # 介面字串 (7073 筆，與官方語言檔一一對應)
```

- 兩個 DLL 以同版本官方語言 DLL 為基礎製作，語系 ID 為 `0x0404` (zh-TW)。
- 翻譯用語與排版規範請參閱 [台灣繁體中文工程用語](GLOSSARY.md)。
- 使用前請確認三個檔案皆已完整下載。

## 🛠️ 安裝方式

### 前置作業

1. 安裝 VMware Workstation Pro。
2. 下載本儲存庫 (`Code` → `Download ZIP`)，或執行：

   ```shell
   git clone https://github.com/LaiYueTing/VMware-zh_TW.git
   ```

3. 將 `zh_TW` 資料夾複製到安裝目錄下的 `messages` 資料夾 (需要系統管理員權限)。預設路徑為：

   ```text
   C:\Program Files\VMware\VMware Workstation\messages\zh_TW
   ```

   > 17.x 版的預設安裝目錄為 `C:\Program Files (x86)\VMware\VMware Workstation`。

完成後，任選下列一種方式指定介面語言。

### 方式一：修改使用者設定檔 (建議)

設定一次即可生效，不受捷徑影響，從開始功能表、工作列或檔案總管開啟皆會套用。

1. 關閉 VMware Workstation。
2. 以文字編輯器開啟 `%APPDATA%\VMware\preferences.ini`。
3. 新增下列設定 (若已有 `pref.locale` 則直接修改其值)：

   ```ini
   pref.locale = "zh_TW"
   ```

4. 存檔後重新開啟 VMware Workstation。

### 方式二：捷徑加入啟動參數

僅透過該捷徑啟動時生效。

1. 在 VMware Workstation 捷徑上按右鍵，選擇「內容」。
2. 在「捷徑」索引標籤的「目標」欄位最後，空一格後加上 `--locale zh_TW`：

   ```text
   "C:\Program Files\VMware\VMware Workstation\vmware.exe" --locale zh_TW
   ```

3. 按「確定」後，透過此捷徑開啟 VMware Workstation。

### 移除方式

1. 刪除 `messages\zh_TW` 資料夾。
2. 移除 `preferences.ini` 中的 `pref.locale` 設定，或移除捷徑上的 `--locale zh_TW` 參數。

## ❓ 常見問題

- **更新主程式後中文消失？**
  升級或修復安裝時，安裝程式可能會清除 `messages` 資料夾，請重新複製對應版本的 `zh_TW` 資料夾。
- **部分介面仍顯示英文？**
  通常是語言檔與主程式版本不符，請參考 [版本對照表](#版本對照表) 下載對應版本。
- **複製檔案時權限不足？**
  請以系統管理員身分執行檔案總管，或在複製時同意 UAC 提示。

## 📄 授權條款

本專案以 [GPL-3.0](LICENSE) 授權條款釋出。VMware 與 VMware Workstation 為 Broadcom 的商標。

[project-url]: https://github.com/LaiYueTing/VMware-zh_TW "GitHub 繁體中文化"
[tags-url]: https://github.com/LaiYueTing/VMware-zh_TW/tags "標籤"

[issues-url]: https://github.com/LaiYueTing/VMware-zh_TW/issues "議題"
[issues-image]: https://img.shields.io/github/issues/LaiYueTing/VMware-zh_TW?style=flat-square&logo=github&label=Issue

[stars-url]: https://github.com/LaiYueTing/VMware-zh_TW/stargazers "星標"
[stars-image]: https://img.shields.io/github/stars/LaiYueTing/VMware-zh_TW?style=flat-square&logo=github&label=Star

[forks-url]: https://github.com/LaiYueTing/VMware-zh_TW/network "分支"
[forks-image]: https://img.shields.io/github/forks/LaiYueTing/VMware-zh_TW?style=flat-square&logo=github&label=Fork

[license-url]: LICENSE "授權條款"
[license-image]: https://img.shields.io/github/license/LaiYueTing/VMware-zh_TW?style=flat-square&logo=github&label=License
