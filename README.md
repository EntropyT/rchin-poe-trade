# Readme.md

![GitHub Releases](https://img.shields.io/github/downloads/rChinnnn/rchin-poe-trade/total)
![GitHub Latest Releases](https://img.shields.io/github/downloads/rChinnnn/rchin-poe-trade/latest/total)
![GitHub Release Date](https://img.shields.io/github/release-date/rChinnnn/rchin-poe-trade)

# rChin POE Trade For CN
POE 快速查价工具 (Built with Electron and Vue.)
> 绝大部分的物品皆可搜寻 - 限定Q服（腾讯服）及国际服(中文化)使用 

### 安装版本说明
* 点选 [Releases页面](https://github.com/EntropyT/rchin-poe-trade/releases)，有两种版本可以下载
    * `rchin-poe-trade-Setup-xxx.exe` 安装版，若程序侦测到有最新版，会在背景下载新版本并在重开程序时更新
    * `rchin-poe-trade-xxx.exe` 绿色版，无法支援自动更新

## 【免责申明】
* **使用此程序者请自行承担所有可能后果和风险**
  * 此程序并无修改任何内存和游戏本体
  * 运作原理为抓取 POE 游戏内对物品复制后的文字进行分析，以利快速查价
  * 调用的 API 皆为官方公开资源，请勿于短时间内快速搜索造成服务器负担
 
## 热键功能
| 按键 | 功能说明 | 
| --- | --- | 
| F5 | 程序显示在最上层，并且透明化 (可漂浮在POE程序上) | 
| F6 | 程序取消在最上层，并取消透明化 | 
| PageUp   | 透明化程度 +5% | 
| PageDown | 透明化程度 -5% | 

**热键注意事项：所有热键于 POE 游戏视窗内皆无作用！必须在工具视窗内才能使用各功能**

## 使用说明
1. 将程序开启
2. 点回 Home 页签
3. 切换视窗回游戏中
4. 将鼠标停在游戏物品上，按下 Ctrl+C 
5. 程序将自动判断此次搜索物品
6. 各类物品有不同设定，详见下列状况

- [非自動搜尋項目](#非自動搜尋項目)
    - [非傳奇裝備](#非傳奇裝備)
- [自動搜尋項目](#自動搜尋項目)
    - [傳奇裝備](#傳奇裝備)
    - [地圖](#地圖)
    - [技能](#技能)
    - [其餘項目](#其餘項目)
- [未支援項目](#未支援項目)

### 非自動搜尋項目

#### 非傳奇裝備
* 預設帶入稀有度：非傳奇
* 預設帶入物品分類
    * 武器可選大類別（Ex: 匕首/單手武器、長杖/雙手武器）
* 預設帶入所有詞綴及數值
    * 欲搜尋的詞綴需自行點選開啟
    * 無隨機數值的詞綴無法輸入最小/最大值
* 勢力裝預設帶入勢力基底
* 物品等級、物品基底、污染為手動選擇項目
* **各選項設定完成後，必須手動按下右下角查詢按鈕**

### 自動搜尋項目

#### 傳奇裝備
* 預設帶入稀有度：傳奇
* 預設帶入物品分類
* 詞綴表格預設不展開，若需篩選特定詞綴可點選物品名稱或"詞綴設定"展開表格
* 支援未鑑定的傳奇裝，但會搜尋到相同基底的其他傳奇
    * 例如：族譜最複雜的皮革腰帶

#### 地圖
* 預設帶入稀有度
    * 傳奇圖：傳奇
    * 其他圖：非傳奇
* 預設帶入地圖基底
* 預設帶入地圖階級
* 預設帶入勢力領域與凋落地區
* 污染為手動選擇項目

#### 技能
* 預設帶入技能品質
* 預設帶入技能基底
* 技能等級、污染為手動選擇項目

#### 其餘項目
* 通貨、卡片、精髓、聖甲蟲、裂片..等其餘物品皆會自動搜尋

### 未支援項目
* 非傳奇藥劑(白/藍水)
* 鍊魔器官

## 其他功能

### 輿圖區域名稱複製
1. 點選開關展開
2. 選擇想搜尋的輿圖區域（點選即複製）
3. 回到輿圖倉庫頁搜尋欄貼上，可快速搜尋各區地圖
![](https://i.imgur.com/loaymoI.png)

## 遊戲內搜尋截圖
### 傳奇物品
#### 一般物品
![](https://i.imgur.com/KlsWdZl.jpg)
### 三相珠寶
![](https://i.imgur.com/tTW2UUm.jpg)

### 稀有裝備
#### 範例1
![](https://i.imgur.com/bQpIr9H.png)
#### 範例2
![](https://i.imgur.com/BSM3Cu9.jpg)

### 技能寶石
#### 一般
![](https://i.imgur.com/DSdGJwz.png)
#### 瓦爾
![](https://i.imgur.com/DFDmXF6.jpg)

### 地圖
#### 塑者
![](https://i.imgur.com/XWD8aCS.png)
#### 尊師(守衛)
![](https://i.imgur.com/1NrkPjP.png)
