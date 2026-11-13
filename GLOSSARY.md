# VMware Workstation Pro 台灣繁體中文工程用語

本文件定義語言檔 (`vmware.vmsg`、`vmui-zh_TW.dll`、`vmappsdk-zh_TW.dll`) 的翻譯用語與排版規範。新增或修改翻譯時，請以本文件為準。

## 📐 排版規範

### 語言

- 一律使用台灣繁體中文 (Traditional Chinese, zh-TW)，不可混用簡體字或中國大陸用語。

### 空格

- 中文與英文單字、半形數字之間保留半形空格：`VMware Tools 未安裝`、`4 GB`。
- 數字與單位之間保留半形空格：`10 Gbps`、`512 MB`。度數 (`90°`) 與百分比 (`15%`) 不加空格。
- 全形標點與其他字元之間不加空格：`無法連線至 %1$s：`。
- 佔位符 (`%1$s`、`%d`) 視同英文單字，前後保留空格：`%1$s 不是允許使用的快速鍵。`
  - 例外：佔位符代表一段完整的前置訊息時 (例如 `%1$s確定要重設虛擬機器「%2$s」嗎？`) 不加空格，與官方語言檔一致。
- 省略號 `...` 前保留半形空格：`瀏覽(&R) ...`。

### 標點符號

- 統一使用全形中文標點：`，` `。` `：` `；` `！` `？`。
- 引號使用直角引號：`「 」` `『 』`。
- 不重複使用標點符號 (禁止 `！！`、`？？`)。
- 括號維持半形並前後留空格：`信賴平台模組 (TPM)`。
- 完整英文句子或特殊名詞內使用半形標點，英文標點後空一格。

### 字元與大小寫

- 數字一律使用半形字元 (`1000`，不可寫成 `１０００`)。
- 專有名詞使用官方大小寫：`VMware`、`ESXi`、`macOS`、`BIOS`、`UEFI`、`IPv6`。

### 快速鍵標記

- 選單與按鈕的快速鍵字母放在字尾括號內，不加空格：`移除(_R)`、`設定(&S) ...`。
- `_X` (vmsg) 與 `&X` (DLL) 需與原字串的快速鍵機制一致，不可互換。

### 格式字串

- 不可增刪或改變佔位符 (`%1$s`、`%2$d`、`%%`、`|0A`、`|22`)，數量與型別需與官方語言檔一致。
- `|0A` 為換行、`|22` 為雙引號、`|7C` 為直線符號，屬於跳脫序列，排版檢查時視為中性字元。

## 🖥️ 虛擬化術語

| English | 台灣用語 | 避免使用 |
| --- | --- | --- |
| virtual machine (VM) | 虛擬機器 | 虛擬機 |
| guest operating system | 客體作業系統 | 虛擬機作業系統、客戶機系統 |
| host | 主機 | 宿主機 |
| hypervisor | Hypervisor | 虛擬機監視器 |
| snapshot | 快照 | |
| take snapshot | 記錄快照 | 拍攝快照、創建快照 |
| revert to snapshot | 還原至快照 | 恢復快照 |
| suspend / resume | 暫停 / 繼續執行 | 掛起 / 恢復 |
| power on / power off | 開機、開啟電源 / 關機 | |
| clone / linked clone / full clone | 複製 / 連結複製 / 完整複製 | 克隆 |
| template | 範本 | 模板 |
| library | 程式庫 | 庫 |
| shared folder | 共用資料夾 | 共享文件夾 |
| shared virtual machine | 共用虛擬機器 | 共享虛擬機 |
| bridged networking | 橋接網路 | 橋接網絡 |
| host-only networking | 僅主機模式網路 | 僅主機網絡 |
| private network | 私人網路 | 專用網路 |
| virtual network adapter | 虛擬網路介面卡 | 虛擬網卡 |
| hardware compatibility | 硬體相容性 | 硬件兼容性 |
| nested virtualization | 巢狀虛擬化 | 嵌套虛擬化 |
| passthrough | 直通 | 透傳 |
| quiesce | 靜止 | 靜默 |
| migrate / migration | 移轉 | 遷移 |
| hosted (product / I/O) | 代管 | 託管、托管 |
| consolidate | 整合 | |
| virtual appliance | 虛擬應用裝置 | 虛擬設備 |
| Trusted Platform Module | 信賴平台模組 (TPM) | 可信平台模塊 |
| datastore | 資料存放區 | 數據存儲 |

## 💾 儲存與裝置

| English | 台灣用語 | 避免使用 |
| --- | --- | --- |
| disk / virtual disk | 磁碟 / 虛擬磁碟 | 磁盤 |
| hard disk | 硬碟 | 硬盤 |
| drive | 磁碟機 | 驅動器 |
| CD/DVD drive | CD/DVD 磁碟機 | 光驅 |
| floppy | 軟碟 | 軟盤 |
| partition | 分割區 | 分區 |
| sector | 磁區 | 扇區 |
| volume | 磁碟區 | 卷 |
| image / ISO image | 映像 / ISO 映像 | 鏡像、圖像 |
| mount | 掛載 | |
| eject | 退出 | 彈出 |
| mirror | 鏡像 | |
| serial port / parallel port | 序列埠 / 並列埠 | 串口 / 並口 |
| bus | 匯流排 | 總線 |
| device | 裝置 | 設備 |
| driver | 驅動程式 | 驅動程序 |
| firmware | 韌體 | 固件 |
| memory | 記憶體 | 內存 |
| hot-add / hot-plug | 熱加入 / 熱插拔 | |
| offload | 卸載 | |

## 🌐 網路與安全性

| English | 台灣用語 | 避免使用 |
| --- | --- | --- |
| network | 網路 | 網絡 |
| protocol | 通訊協定 | 協議 |
| client | 用戶端 | 客戶端 |
| server | 伺服器 | 服務器 |
| proxy | Proxy / Proxy 伺服器 | 代理 |
| port | 連接埠 | 端口 |
| socket | 通訊端 | 套接字 |
| address | 位址 | 地址 |
| domain name | 網域名稱 | 域名 |
| tunnel | 通道 | 隧道 |
| certificate | 憑證 | 證書 |
| signature | 簽章 | 簽名 |
| revocation | 撤銷 | |
| credentials / Credential Manager | 認證 / 認證管理員 | 憑據 |
| ticket | 票證 | |
| hash | 雜湊 | 哈希 |
| key (license / encryption) | 金鑰 | 密鑰 |
| algorithm | 演算法 | 算法 |
| identity | 身分 | 身份 |
| authentication | 驗證 | 認證 (指流程時) |

## 🧰 軟體與介面

| English | 台灣用語 | 避免使用 |
| --- | --- | --- |
| user | 使用者 | 用戶 |
| account | 帳戶 | 賬戶、賬號 |
| default | 預設 | 默認 |
| settings / preferences | 設定 / 偏好設定 | 設置 |
| configuration file | 設定檔 | 配置文件、設定檔案 |
| file / folder / directory | 檔案 / 資料夾 / 目錄 | 文件 / 文件夾 |
| information / message | 資訊 / 訊息 | 信息 / 消息 |
| software / hardware | 軟體 / 硬體 | 軟件 / 硬件 |
| application | 應用程式 | 應用程序 |
| process | 處理程序 | 進程 |
| thread | 執行緒 | 線程 |
| operation | 作業 | 操作 |
| apply | 套用 | 應用 |
| policy | 原則 | 策略 |
| support | 支援 | 支持 |
| compatible | 相容 | 兼容 |
| enable / disable | 啟用 / 停用 | 激活 / 禁用 |
| create | 建立 | 創建 |
| change / modify | 變更 / 修改 | 更改 |
| view | 檢視 | 查看 |
| visit (website) | 造訪 | 訪問、存取 |
| contact | 聯絡 | 聯繫 |
| wizard | 精靈 | 嚮導、向導 |
| dialog box | 對話方塊 | 對話框 |
| menu / toolbar / tab | 選單 / 工具列 / 索引標籤 | 菜單 / 工具欄 / 選項卡 |
| control | 控制項 | 控件 |
| hotkey | 快速鍵 | 熱鍵 |
| key combination | 按鍵組合 | 鍵組合 |
| Spacebar | 空白鍵 | 空格鍵 |
| aspect ratio | 長寬比 | 縱橫比 |
| user interface | 使用者介面 | 用戶界面 |
| interactive | 互動式 | 交互式 |
| terminal | 終端機 | 終端 |
| back (wizard) | 上一步 | 返回 |
| return (a value) | 傳回 | 返回 |
| screenshot | 螢幕擷圖 | 截圖、截屏 |
| registry key | 登錄機碼 | 註冊表項 |
| save as | 另存新檔 | 另存為 |
| plan / program | 計畫 | 計劃 |
| consistency | 一致性 | 相同性 |
| license agreement | 授權合約 | 授權協議 |
| serial number | 序號 | 序列號 |
| hyphen / dash | 連字號 | 破折號、短劃線 |
| crash | 當機 | 崩潰 |
| exception | 例外 | 異常 |
| implement / implementation | 實作 | 實現 |
| text | 文字 | 文本 |
| asynchronous | 非同步 | 異步 |
| recursive | 遞迴 | 遞歸 |
| loop | 迴圈 | 循環 (指程式迴圈時) |
| binary / hexadecimal | 二進位 / 十六進位 | 二進制 / 十六進制 |
| escape character | 跳脫字元 | 轉義符 |
| non-maskable interrupt (NMI) | 不可遮罩式中斷 | 不可屏蔽中斷 |
| optimize | 最佳化 / 優化 | 优化 |
| printer | 印表機 | 打印機 |
| database | 資料庫 | 數據庫 |

## ✅ 檢查清單

提交翻譯前請確認：

1. 鍵值數量與順序與官方語言檔 (`messages/ja/vmware.vmsg`) 一致。
2. 每個字串的佔位符與官方語言檔一致。
3. 沒有簡體字、全形英數字與上表「避免使用」欄位中的用語。
4. 符合上方的排版規範。
5. DLL 的語系 ID 為 `0x0404` (圖示與 PNG 等非文字資源維持 `0x0409`)，版本資訊的 `InternalName`、`OriginalFilename` 為 `*-zh_TW`。
