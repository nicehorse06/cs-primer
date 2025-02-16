# 資訊科學學習入門

## 文章目標
* 以資訊科學為志願的學生
* 內容除了書以外都是免費的

## 簡易流程
* 註冊ChatGPT，有問題直接問
* 註冊Github帳號
* 下載VScode
* 學習git
* 學習操作Linux(可以的話)
* 依據興趣選擇一門程式語言
* 依據興趣學習資訊科學相關的知識

## 目標參考
* 開源一個讓大家用起來很方便的程式，獲得星星關注
* 看到自己常用的開源程式有issue，試著解決，成為貢獻者
* 把學習筆記紀錄在Github Issue Blog或是專案
* 藉由Github page建立個人網站
* 在Leetcode刷題，讓自己更熟悉資料結構與演算法
    * 如果有興趣可繼續準備APCS或是當資訊競賽的選手
* 做Line的聊天機器人

## git
* 一種文字檔案的版本控管程式
* 可以使用VScode/Linux命令行/圖形化支援工具來使用
* 建議用VScode入門，能力所及就了解Linux命令行
  

## Github
* it程式的儲存庫網站，有程式的每次修改紀錄
* 可以用git程式做版本控管並儲存程式碼
* 可以免費的建立個人網頁
* 可以寫技術部落格
* 可以參與其他人的程式碼
* 提供免費自動化服務，比如自動測試寫完的程式碼



## VScode
* VScode是資訊界主流的編輯器，專門處理文字
* 很多網友寫對應的套件幫助開發
    * 比如為了Python寫語法補全套件
* 用的人多所以遇到問題好解決
* 因為跟寫網頁是同一種技術，所以甚至連Github網頁也提供VScode編輯界面

## Linux操作
### 簡介
* 業界主流的開源作業系統
* 方便的用命令行控制電腦
* Linux是作業系統的核心(Kernel)，各廠商會依據核心發展出自己的Linux發行版(distribution)
    * 這裡推薦使用Ubuntu，方便上手，也是免費的
    * 我們實際會用到的Linux都是Linux發行版

### 優勢，為什麼要學Linux
* 有眾多開發者提供的免費開發工具
* 有免費Linux可以直接下載安裝
* 可以穩定運行在舊筆電上，廢土變黃金
* Linux以文字命令行操作為主
    * 好做學習筆記，學一次不會變
    * 用文字代表可以方便寫成腳本操作，讓電腦控管自己
* 因為開源，有眾多開發者一起檢視問題，不容易中毒
* 少掉不必要的圖形界面，當程式出錯時方便找出問題
    * 比如為什麼沒有編譯成功或是設定Python執行路徑

### 劣勢
* 學習門檻高，一般使用者習慣windows界面
* 安裝門檻高，要安裝Linux虛擬機/實體機
* 要持續學習，Linux出錯會噴一些錯誤訊息，要去網路上或GPT找出問題
* 支援遊戲少，不完美支援Windows辦公室軟體，有些設備不支援Linux

### 命令行範例
* 以移動檔案/重新命名檔案/展示資料夾所有檔案為例
  * Windows移動檔案是用滑鼠拖拉到其他地方
  * Windows重新命名是右鍵重新命名
  * Windows展示資料夾所有檔案是點開資料夾，如果想看隱藏檔案，要去我的電腦中做設置
* 以下為Linux中的範例
  * `$`僅表示現在的權限為一般使用者在下命令

``` sh
# 移動檔案
# 表示把現在路徑下的this_file，移動到資料夾new_dir，之後路徑變new_dir/this_file
$ mv this_file new_dir/

# 重新命名
# 移動指令同時可改名，把old_file_name檔名改成new_file_name
$ mv old_file_name new_file_name

# 展示目前資料夾下所有檔案
$ ls

# 展示所有檔案細節，包含隱藏檔案
# 一樣的命令，用參數即可調整功能，不用額外背操作
# -la為功能參數，-a代表連隱藏檔都要看，-l代表要看更多細節如權限/擁有者/創建日期
# 用 man ls，就可以知道ls的所有參數用法
$ ls -la

# 命令行百百種，初期學基本操作就好，不知道功能問GPT
# 如 ls, cd, pwd, cp, rm, cat, mv , touch, mkdir, man, sudo.
```
### 取得Linux操作環境
* 瀏覽器可在用[JSLinux](https://bellard.org/jslinux/)
* APP可以下載Termux
* 在實體筆電上安裝Ubuntu
  * 可選[雙系統](https://www.youtube.com/watch?v=yMHOpOuyjdc)
    * 如果安裝時把windows的空間刪掉就是單系統
  * 安裝流程大致如下:
    * 從Ubuntu網站下載[Ubuntu Desktop](https://ubuntu.com/download/desktop) ISO檔
    * 準備一個隨身碟當開機碟
    * 下載Rufus把Ubuntu放到隨身碟中變為開機碟
    * 如果要設定雙系統要進行磁碟切割(可選)
    * 去Google搜尋一下筆電廠牌開機時用什麼按鍵進入BIOS，如Lenovo用F1
    * 插上開機碟，重開機時進入BIOS選擇剛剛插入的隨身碟開機
    * 進入Ubuntu安裝畫面後，就依據指引填資料，安裝結束就得到一台Ubuntu電腦
* 在virtualbox上安裝Ubuntu虛擬機，參考[教學](https://www.youtube.com/watch?v=Hva8lsV2nTk)
* 在Windows上安裝WSL，參考[教學](https://www.youtube.com/watch?v=fucKUKsv7Q4)

### 學習
*  [鳥哥的Linux私房菜](https://linux.vbird.org/)
*  在命令行上用man就可以知道指令用法
*  [archlinux document](https://archlinux.org/)

### 作業系統比較
#### MacOS
* MacOS跟Linux操作界面相似，所以MacOS是工程師開發的主流
* MacOS專為蘋果電腦而生，所以運行效率/省電/畫面流暢都比較好
* MacOS在個人電腦使用上不輸Linux，除了價錢

#### Windows
* Windows的操作以圖形化界面操作為主
* 每個圖形化軟體，使用者都要記得不同的畫面位置操作
* Linux以文字命令行為主，學一次就不會變，並且命令間可以組合
* Windows會有效能問題，用久會卡會頓，這跟它沒有開源有關
* Windows不便宜，對Linux熟練者來說，Windows唯一優勢是打遊戲跟使用Word

#### 比較的結論
* 以穩定開發的工程師來說Macbook是首選，穩定且蓄電長
* 用Windows/Macbook筆電連線Linux的伺服器做開發
    * 這是最折衷的使用方式
    * 伺服器可以是另一台實體電腦，或是裝在同一台電腦的虛擬機
* 以Linux出廠的電腦比較少，通常都是拿二手Windows重灌成Linux
    * 以Linux當作主要開發的電腦學習，可以成長很多
    * 建議用Ubuntu入門，Ubuntu的操作跟安裝都友善，也是主流

## 語言選擇
> 不管學什麼程式語言，英文才是最重要的
> 有什麼問題GPT大多能回答

### C
* 可以精準學習基本資訊科學知識，如記憶體管理/資料結構/作業系統
* 可以用來開發/學習Linux kernel
  * 所謂的嵌入式工程師，也是開發Linux相關應用
  * 台灣軟體業薪水最高的大概是寫C的工程師
  * C大概是壽命最常的語言
* 推薦可以先學C，可能有點難，是因為他被設計來寫作業系統的，如Linux是C寫的
* 資源
  * [The C Programming Language, 2/e ](https://www.tenlong.com.tw/products/9780131103627)
  * [C 語言入門影片課程](https://www.youtube.com/watch?v=yWPGumB64tM&list=PLY_qIufNHc293YnIjVeEwNDuqGo8y2Emx)
### C++
* 用來寫高效率的程式
  * 遊戲的高效能引擎通常用C++
* 學生的程式競賽C++是主流
* C vs C++
  * C++相比C多了很多進階語法跟內建套件，所以很好的管理程式
  * 但因為套件語法多了，每個人寫法不一樣容易出錯，故需要穩定的程式如作業系統選C
### Python
* 語法簡單，如果想要快速學一門語言，Python是首選
* 如果是要開發AI/伺服器應用/聊天機器人，選Python
### JavaScript
* 如果想要做一個自己的專屬網站，選JavaScript
  * 做網站的視覺少不掉還要學HTML(文字), CSS(樣式)


## 資訊科學學科(TODO)
 *  [計算機概論](https://www.youtube.com/watch?v=EDYjPpn1OmE&list=PLil-R4o6jmGiDc1CC8PyBbasl8kR9r8Wr)
 * 基本資料結構知識
 * 基本作業系統知識
 * 基本演算法


## Linux原始碼學習(TODO)
 
### Jserv課程
* 加入Jserv的課程社團 [2025 年系統軟體系列課程討論區](https://www.facebook.com/groups/system.software2025/)
  * [成功大學資工系(所) Wiki 系統](https://wiki.csie.ncku.edu.tw/Homepage)
  * Jserv的專長主要在OS/硬體/Linux/系統底層開發
* [youtube](https://www.youtube.com/@sysprog/videos)，老師都是線上課程


## 如何在申請大學加分(TODO)
* 貢獻知名原始碼，獲得專案維護者的認可
* 在某一個國際會議做講者