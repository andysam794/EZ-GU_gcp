# EZ-GU 看股選股評估服務
## Big Data巨量資料分析就業養成班(BDSE25) -第四組專題成果

### 免責聲明: 此系統之數據、圖表、運算結果等所有產出，皆僅是學術練習用途，不可作為投資等其他所有商業行為之依據或應用。若任意使用本專題內容之成果於投資等其他所有商業行為而造成利益損害，我方並不會負任何責任。

### 目錄

- [專題構思](#專題構思)
- [目標特色](#目標特色)
- [功能概述](#功能概述)
- [網頁開發架構](#網頁開發架構)
- [前往預覽](#前往預覽)

 

## 專題構思:

　　市面上充滿著各式各樣的看股工具及其衍生的服務，而這些服務所提供的指標與延伸服務，讓使用者通常需要兼用2~3個工具才能滿足看股的資訊需求量。本專題經由組內兩位股市達人發想，透過1.七大看股指標互動式圖像化，2.投資組合評估工具，3.五項選股推薦，4.指標預測模型，來達到EZ-GU(股)，EZ-GU(顧)的服務目的，讓單一服務滿足大部分的需求。

　　透過本次專題，可讓每位組員都能”實做”到課程中所學的，資料爬取、資料清洗、資料處理運算、資料庫建置、資料庫寫入、Hadoop叢集架設、機器學習模型訓練建置、後端\資料庫連接、前端\後端連接、前端畫面呈現等技能，達到學以致用並累積實做經驗的目的。


## 目標特色:

1.七大看股指標互動式圖像化  
2.投資組合評估工具  
3.四項選股推薦  
4.指標預測模型  

<p align="right">(<a href="#top">back to top</a>)</p>



## 功能概述:

## 七大看股指標互動式圖像化：

　　由擁有股市knowhow的組員們挑選出七大常用指標，透過api以及爬蟲技術，爬取股票id以及指標所需的股市資料，並進行運算清洗得到一個DF，最後將其寫入資料庫中，讓後端抓取資料庫資料回傳給前端進行繪圖呈現。
七大指標：[K線、漲跌幅、布林通道、RSI、MACD、KDJ、OBV]。


## 投資組合評估工具：

　　由使用者自行輸入"交易日期"及 "購買資訊"，收到前端的請求後，後端會進到資料庫與連接api抓取運算所需要的資訊，完成運算後會回傳當前使用者的投資組合曝險程度及當前報酬率資訊，提供使用者評估現有投資組合或模擬投資組合效益之功用。


## 四項選股推薦：

-依照「投信購買標的」提供投資人購買方向。  
-依照「週轉率排行」提供當沖、週轉率較高等適合當沖標的族群。  
-依照VCP「波動收縮規律」設定參數，間接從台灣股市挑選出中長線股票。  
-依照「技術指標」提供喜好運用KD、MACD、RSI作為買入或賣出的基準。  

<p align="right">(<a href="#top">back to top</a>)</p>



## 網頁開發架構：

```
EZ-GU_gcp
|__ run.py: 啟動app
|__ requirements.txt: all python package
|__ app
    |__ __init__.py: all route
    |__ static
    |   |__ css
    |   |   |__ css files
    |   |       ...
    |   |       ...
    |   |__ img
    |   |   |__ image files
    |   |       ...
    |   |       ...
    |   |__ js
    |   |   |__ javascripts files
    |   |       ...
    |   |       ...
    |   |__ lib
    |       |__ template for css files
    |           ...
    |           ...
    |
    |__ templates: all html files
        |__ index.html: 系統首頁(七大指標)
        |__ about.html: 專題介紹頁
        |__ widget.html: 四項選股推薦頁
        |__ ByS_Ranking.html: 選股資訊子頁-券商買賣排行
        |__ Margin_Trading_and_Short_Selling.html: 選股資訊子頁-融資融券排行
        |__ EPS.html: 選股資訊子頁-EPS
        |__ form.html: 投資組合頁
        |__ parts: 模板block
            |__ base.html: 基礎頁面
            |__ to_name.html: 選股資訊子頁-基礎頁面
            |__ 404.html: 404頁面
```

<p align="right">(<a href="#top">back to top</a>)</p>


## 前往預覽：

- <p align="left">(<a href="http://34.81.90.168" target="_blank">Website link</a>)</p>

<p align="right">(<a href="#top">back to top</a>)</p>