# 📌 資訊科學學習入門

## 🎯 文章目標
- 以資訊科學為志願的學生
- 內容除了書以外都是免費的

## 🔄 簡易流程
1. 註冊 ChatGPT，有問題直接問
2. 註冊 GitHub 帳號
3. 下載 VSCode
4. 學習 Git
5. 學習操作 Linux（如果可以）
6. 依據興趣選擇一門程式語言
7. 依據興趣學習資訊科學相關的知識

## 🎯 目標參考
- 開源一個讓大家用起來很方便的程式，獲得 Star 關注
- 看到自己常用的開源程式有 issue，試著解決，成為貢獻者
- 把學習筆記記錄在 GitHub Issue Blog 或專案中
- 使用 GitHub Pages 建立個人網站
- 在 Leetcode 刷題，熟悉資料結構與演算法
  - 如果有興趣可準備 APCS 或參加資訊競賽
- 開發 Line 聊天機器人

---

## 🛠 Git
> **沒有用git開發的軟體工作千萬不要去 !**

- 一種文字檔案的版本控管程式
- 可以使用 VSCode / Linux 命令行 / 圖形化工具來操作
- **建議：** 先用 VSCode 入門，之後學習 Linux 命令行
- **參考資源：**
  - 📖 [為你自己學 Git](https://gitbook.tw/)
  - 📖 [Git 基礎中的基礎指令](https://github.com/nicehorse06/se-job/blob/master/interview/git/basic_intro.md)

---

## 🏠 GitHub
> **GitHub 就是工程師的 Facebook！**

- 程式碼的儲存庫，保留每次修改紀錄
- 透過 Git 版本控管儲存程式碼
- 可以免費建立個人網頁
- 可以寫技術部落格
- 可參與其他人的開源專案
- 提供 **免費自動化服務**，如 **自動測試程式碼**

---

## 📝 VSCode
- VSCode 是資訊界的主流編輯器，專門處理文字
- 擁有大量擴充套件，如：
  - **Python** 補全語法
  - **Git** 版本管理
- **好處：** 使用者多，遇到問題容易找到解決方案
- **與 GitHub 整合良好**，甚至可以用 VSCode 編輯 GitHub Pages

---

## 🐧 Linux 操作
### 🏗 簡介
* 業界主流的開源作業系統
* 方便的用命令行控制電腦
* Linux是作業系統的核心(Kernel)，各廠商會依據核心發展出自己的Linux發行版(distribution)
    * 這裡推薦使用Ubuntu，方便上手，也是免費的
    * 我們實際會用到的Linux都是Linux發行版

### 優勢，為什麼要學Linux
- 擁有免費開發工具，許多工具只在 Linux 上運行
- 可以運行在舊筆電上，將廢土變黃金
- **命令行操作優勢**
  - 可用文字記錄筆記，學習不會過時
  - 文字命令可轉換成自動化腳本
- **開源社群審核安全性，不易中毒**
- **錯誤訊息易於 Debug**
* 少掉不必要的圖形界面，當程式出錯時方便找出問題
    * 比如為什麼沒有編譯成功或是設定Python執行路徑

### ❌ Linux 劣勢
- **學習門檻高**：需要適應命令行
- **安裝門檻高**：需安裝 Linux 虛擬機或雙系統
- **需要持續學習**：出錯時需查詢解決方案（如 GPT、Google）
- **遊戲支援少**，部分 Windows 軟體無法運行


### 命令行範例
* 以移動檔案/重新命名檔案/展示資料夾所有檔案為例
  * Windows移動檔案是用滑鼠拖拉到其他地方
  * Windows重新命名是右鍵重新命名
  * Windows展示資料夾所有檔案是點開資料夾，如果想看隱藏檔案，要去我的電腦中做設置
* 以下為Linux中的範例
  * $僅表示現在的權限為一般使用者在下命令

sh
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


---

## 🔍 語言選擇
> **無論學什麼語言，英文最重要！**
> **有問題？GPT 幾乎都能回答！**

### 🔷 C 語言
- 學習基本計算機概念（記憶體管理、資料結構、作業系統）
- 用於開發 Linux Kernel 和嵌入式系統
- 台灣薪水最高的軟體工程師大多寫 C
- **推薦資源：**
  - 📖 [The C Programming Language, 2/e](https://www.tenlong.com.tw/products/9780131103627)
  - 🎥 [C 語言入門影片](https://www.youtube.com/watch?v=yWPGumB64tM&list=PLY_qIufNHc293YnIjVeEwNDuqGo8y2Emx)

### 🔷 C++
- **高效能應用**：如 **遊戲引擎、圖形處理**
- **資訊競賽主流語言**
- **與 C 比較**
  - C++ **有物件導向設計**，管理程式較容易
  - C **較低階但更穩定**，適合開發系統級程式

### 🔷 Python
- **簡單易學**，適合初學者
- **適合應用場景**
  - **AI / 機器學習**
  - **Web 伺服器開發**
  - **聊天機器人**

### 🔷 JavaScript
- **適合開發 Web 應用**
- 需搭配 **HTML（內容）、CSS（樣式）**

---

## 🏛 資訊科學學科
> 其實計算機上的知識不難，只是義務教育沒教
> 資工系的必修們其實都不是在教如何寫程式，可以簡略濃縮成數學/軟硬體整合/優化程式時間和空間的知識
> 只會程式語言也可以馬上工作，但會的很淺像是刷油漆，但能養活自己，而資工的知識是為了蓋大樓，可以用一輩子
> 可以先有一個專案目標，然後覺得不足，再去學習這些知識


### 計算機概論
* [計算機科學領域地圖(開中文字幕)](https://www.youtube.com/watch?v=SzJ46YA_RaA)
* [計算機概論](https://www.youtube.com/watch?v=EDYjPpn1OmE&list=PLil-R4o6jmGiDc1CC8PyBbasl8kR9r8Wr)
* 
### 📂 資料結構
- 決定 **如何存取和管理資料**
* 以下範例是兩種資料結構的類比
  * 當要查閱cherry是第幾筆時
    * 1號資料看一眼就知道是第三筆
    * 2號資料要從頭數，數到最後才知道
  * 當要新增資料orange到位置2時
    * 1號資料新增完2.orange，還要把後面的2.banana改成3.banana，3.cherry改成4.cherry
    * 2號資料只要去第2筆新增一筆 * orange
  * 當以查詢為主的程式時，用1號資料方式儲存
  * 當修改資料很頻繁時，用2號資料方式儲存
``` md
## 1號資料
1. apple
2. banana
3. cherry

## 2號資料
* apple
* banana
* cherry
```

### ⚡ 演算法
- **最佳化程式的時間與空間**
* 以經典的範例為例，把資料從台北傳到高雄，n是筆數
  * 1. 使用網路傳資料，時間方程為 `t = n`
  * 2. 開卡車。時間方程為 `t = 10000`
  * 兩者都是資料傳輸的演算法
  * 資料少時會用網路
  * 資料多到一定程度時會改用卡車載資料
* 工程師會因應場景使用適合的演算法

### 作業系統
* todo

---

## 🏗 Linux 原始碼學習（TODO）
### 🎓 Jserv 課程
- **2025 年系統軟體系列課程討論區**
  - [Facebook 社團](https://www.facebook.com/groups/system.software2025/)
  - [成功大學資工 Wiki](https://wiki.csie.ncku.edu.tw/Homepage)
- 📺 [Jserv YouTube 頻道](https://www.youtube.com/@sysprog/videos)

---

## 🎓 如何在申請大學加分（TODO）
- 貢獻知名開源專案，獲得 Maintainer 認可
- 在國際技術會議擔任講者
