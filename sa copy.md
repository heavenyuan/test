### 評估

    - 引用技術
        - 使用Vue2 or Vue3
        - NUXT
    - 功能分析
    - 開發時間
    - 分工

### 套版

    - html搬移
    - sass整理
    - animation js整理

# 各單元



### Adminxxx

    - 登入帳號 <API>

    - 後台帳號登入系統後有需要設定多久時間自動登出
        * 後台完全沒操作30分鐘會自動登出
        * 客服若切換離線按鈕 , 則不列入登出計時

    - 點擊頭像
        - 頭像Logo
        - 選單介面 <視窗> 
            - Upload new image <視窗>
                - 系統默認頭像
                - 選擇上傳圖片 <API>
                    * png , jpeg , jpg
                    * 60px * 60px
                - Clear
                    - 清除上傳圖片
                - 確認按鈕
                    - 上傳圖片 <API>
                - 關閉按鈕
            - Remove image <視窗>
                - 確認按鈕
                    - 移除個人前台顯示照片 <API>
                    * 提示文字：Are You Sure Remove image?
                - 關閉按鈕
            - Change name <視窗>
                - 確認按鈕
                    - 修改前台顯示名稱 <API>
                    - 文字不可空白
                        * 未填寫提示文字：This field is required.
                - 關閉按鈕
            - Change password <視窗>
                - Old Password
                    * 輸入錯誤舊密碼, 提示文字：Old password is failed.
                    * 必填欄位, 未填寫提示文字：This field is required.
                - Ｎew Password
                    * 必填欄位, 未填寫提示文字：This field is required.
                    * 規則：6-20英數字組成 , 格式錯誤提示文字：Password must be 6~20 characters with letters and numbers
                - Confirm Password
                    * 必填欄位, 未填寫提示文字：This field is required.
                    * 與新密碼輸入不同提示：Please enter the same value again.
                - 確認按鈕
                    - 修改登入後台密碼 <API>
                    - 新舊密碼相同 , 提示文字：Ｎew Password is the same as old password.
                - 關閉按鈕
        - 關閉按鈕

### Dashboard

    - Marketing
        - 下拉式選項 <API>
    
    - Real time
        - 資料顯示 <API>

    - Today
        - 資料顯示 <API>

    - Last 7 days
        - 資料顯示 <API>

    - 分析圖
        - Canvas
        - 過去一週圖表 <API>
        - 點擊項目顯示該項目分析圖？

    - 統計說明
        - 相同帳號登出在登入重新聊天，算兩次以此類推

### 聊天室

    - API
        - chats 共 21 支
        - chats-client 共 10 支

    - 聊天室選單
        - 列表 <API>
            - 數量管理
            - 排序管理 <API>
            - 收合
            - 聊天室
                - 客戶資訊顯示 <API>
                - 等候時間
                - 聊天狀態管理 <API>
                - 關閉鈕顯示
                - 關閉資料至歷史紀錄 <API>
                - 判斷00:00:00自動清空
        - 離線狀態
            - 左側聊天列表反灰

    - 資訊區塊
        - 切換顯示Profile、Report
        - Profile
            - Remark
                - 資料顯示 <API>
                - EDIT
                    - 編輯該筆資料 <視窗>
                    - 確認 <API>
                        - 更新列表 <API>
                    - 取消
            - General
                - 資料顯示 <API>
            - Summary
                - 資料顯示 <API>
            - Bank
                - table
                - 資料顯示 <API>
                - EDIT
                    - 編輯該筆資料 <視窗>
                    - 確認 <API>
                        - 更新列表 <API>
                    - 取消
            - Balance
                - 資料顯示 <API>
            - Technology
                - 資料顯預設顯示10筆示 <API>
        - Report
            - Bet
                - table
                    - 排序
                    - 分頁
                    - 顯示總筆數
                    - 小計
                    - 切換顯示筆數
                        * 可選擇2、3、5、10
                        * 預設顯示10筆
                    - 資料顯示 <API>
                    - View按鈕
                        - 開啟Report Detail
                - Report Detail <視窗>
                    - table
                        - 排序
                        - 分頁
                        - 小計
                        - 顯示總筆數
                        - 資料顯示 <API>
                        - View按鈕
                            - 查看詳細資料，點擊另開分頁
                - 分頁
                    - 資料顯示 <API>
            - Transfer
                - Status
                    - 下拉式選單
                    * 包含All、Pending、Success、Fail
                - table
                    - 排序
                    - 分頁
                    - 顯示總筆數
                    - 切換顯示筆數
                        * 可選擇2、3、5、10
                        * 預設顯示10筆
                    - 資料顯示 <API>
                    - Action按鈕
                        - 彈跳視窗 <視窗>
                        - ？
            - Deposit
                - Status
                    - 下拉式選單
                    * 包含All、Pending、Approved、Disapproved
                - table
                    - 排序
                    - 分頁
                    - 顯示總筆數
                    - 小計
                    - 切換顯示筆數
                        * 可選擇2、3、5、10
                        * 預設顯示10筆
                    - 資料顯示 <API>
            - Withdrawal
                - Status
                    - 下拉式選單
                    * 包含Pending、On Hold、Rejected、Verified、Reverted、Disapproved、Processing、Approved
                - table
                    - 排序
                    - 分頁
                    - 顯示總筆數
                    - 小計
                    - 切換顯示筆數
                        * 可選擇2、3、5、10
                        * 預設顯示10筆
                    - 資料顯示 <API>
            - Adjustment
                - table
                    - 排序
                    - 分頁
                    - 顯示總筆數
                    - 切換顯示筆數
                        * 可選擇2、3、5、10
                        * 預設顯示10筆
                    - 資料顯示 <API>
            - Bonus
                - Status
                    - 下拉式選單
                    * 包含All、Inactive、Active、Complete、Return to main、Suspend、Expired、Auto force serve、Manual force serve
                - table
                    - 排序
                    - 分頁
                    - 顯示總筆數
                    - 小計
                    - 切換顯示筆數
                        * 可選擇2、3、5、10
                        * 預設顯示10筆
                    - 資料顯示 <API>
                    - Action
                        - 點擊解除流水限制
                    - View
                        - 點擊查看細項
                    - 細項
                        - ？

    - 功能按鈕
        - 收合
        - Stop this chat <視窗>
            - 確認 <API>
            - 取消
            - 關閉聊天送出問卷
                - 多選模組？ <API>
        - Transfer chat <視窗>
            - 轉移聊天 <API>
            - 確認 <API>
            - 取消
        - Ban customer <視窗>
            - 分類 <API>
            - 禁言天數
            - 禁言備註
            - 確認 <API>
            - 取消

    - 聊天視窗
        - 用戶名稱 <API>
        - 開始時間
        - 問候語 <API>
        - 客服回覆開始計算聊天時間
        - 舊的對話紀錄 <API>
        - 對話 <API>
            - 客服左側
            - 客戶右側
            - 頭像
            - 時間
            - 訊息內容
            - 發送成功打勾 <API>
            - 已讀打勾 <API>
        - 輸入框
            - 預設文字
            - 送出 <API>
            * 預設點擊Enter鍵跟Send鍵都可以發送訊息
        - 快速回覆 <視窗>
            - 分類資料 <API>
            - 選擇文字取代輸入框
        - 迴紋針
            - 上傳 <API>
            * 包含全部的文件、圖片檔跟影像檔 (.bmp 、.jpg、.jpeg、.png、.gif)
        - 表情符號 <視窗>
            - 分類 <API>
            - 送出 <API>
        - 離線狀態
            - 離線狀態無法聊天
            - 聊天對話框反灰        
        - 超過時間未回覆
            - 提示文字：Chat archived due to * minutes of inactivity Close this window.
            - 依據設定的分鐘數顯示
            - 對話視窗反灰，聊天記錄歸欓至歷史對話紀錄 <API>
        - 客結束聊天室狀態
            - 結束聊天室，顯示關閉時間
                - 客服名稱：關閉聊天視窗：關閉時間 Ex. Agent1 closed the chat : 10:50:30 am
            - 前台客戶填寫完聊天後問卷顯示問券結果 <API>
            - 訊息輸入框對話框反灰
        - 設定黑名單聊天頁面
            - 提示文字：Chat archived because customer was banned by wuabby01 for * day
                * 依據設定的天數顯示
            - 聊天列表客戶名單反灰

    - 離線狀態
        - 頁面提示文字：You are currently not accepting chats.

### Traffic

    - filter 控制項
        - Username
            * 輸入框
            * 預設文字：Username
        - Marketing
            * 下拉式選項
        - Language
            * 下拉式選項
        - Actions
            * 下拉式選項
        - Status
            * 下拉式選項
        - Agent
            * 搜尋下拉式選項
            * 預設文字：Select agent
        - IP
            * 輸入框
    - Search按鈕
        - 點擊後，使用設置的選項條件，頁面刷新 <API>
    - Refresh按鈕
        - 每分鐘自動刷新，倒數時間未到可以手動點擊刷新按鈕，時間重新由59秒開始倒數

    - 一般客服頁面
        - table
            - 排序
            - 分頁
            - 顯示總筆數
            - 小計
            - 切換顯示筆數
                * 可選擇2、3、5、10
                * 預設顯示10筆
            - 資料顯示 <API>
            - Username
                - 點擊另開分頁 <視窗>
                    - 顯示Profile、Report資料
                    - 關閉按鈕

    - 客服主管頁面
        - table
            - 排序
            - 分頁
            - 顯示總筆數
            - 小計
            - 切換顯示筆數
                * 可選擇2、3、5、10
                * 預設顯示10筆
            - 資料顯示 <API>
            - Action
                - Start Chat
                    - 點擊進入聊天室頁面，始與用戶聊天
                - Assign
                    - 主管權限可以將在排隊的客戶指派給客服
                    - 點擊彈跳視窗 <視窗>
                        - 顯示所有客服列表 <API>
                            - 顯示客服目前聊天數量
                            - Choose按鈕
                                - 被點選客服目前正在聊天，該用戶則列入Chat Queue名單 <API>
                        - 關閉按鈕
                - Supervise Chat
                    - 點擊進入該聊天室監控
                - Go to Chat
                    - 點擊進去聊天室
                - X
                    - 點擊離開監控的聊天室
                    - 活動狀態由為Supervised 變回Chatting

### Report

    - Agents performance
        - filter 控制項
            - Date
                * 下拉式選項
            - Agent
                * 搜尋下拉式選項
                * 預設文字：Select agent
            - Marketing
                * 下拉式選項
        - Search按鈕
            - 點擊後，使用設置的選項條件，頁面刷新 <API>
        - 頁面資料顯示 <API>
        - Export CSV按鈕
            - 點擊依頁面選擇的欄位匯出csv檔
        - Columns
            * 下拉式勾選項
            * 選擇後，下方表格依據篩選後顯示結果
        - Save按鈕
            - 保存顯示欄位 <API>
            * 保存成功提示文字：Save Success !
            * 保存失敗提示文字：Save Fail !
        - table
            - 排序
            - 分頁
            - 顯示總筆數
            - 小計
            - 切換顯示筆數
                * 可選擇2、3、5、10
                * 預設顯示10筆
            - 表單資料顯示 <API>

    - Archives
        - filter 控制項
            - Category
                * 下拉式選項
            - Username
                * 輸入框
                * 預設文字：Username
            - Agent
                * 搜尋下拉式選項
                * 預設文字：Select agent
            - Marketing
                * 下拉式選項
            - IP
                * 輸入框
            - Login Time
                * 下拉式選項
                - 選擇custom period，展開時間選擇器，最久可以查詢到180天前的資料
        - Search按鈕
            - 點擊後，使用設置的選項條件，頁面刷新 <API>
        - Export CSV按鈕
            - 點擊依頁面選擇的欄位匯出csv檔
        - Columns
            * 下拉式勾選項
            * 選擇後，下方表格依據篩選後顯示結果
        - Save按鈕
            - 保存顯示欄位 <API>
            * 保存成功提示文字：Save Success !
            * 保存失敗提示文字：Save Fail !
        - table
            - 排序
            - 分頁
            - 顯示總筆數
            - 小計
            - 切換顯示筆數
                * 可選擇2、3、5、10
                * 預設顯示10筆
            - 表單資料顯示 <API>
            - View按鈕
                - 點擊顯示歷史聊天對話視窗、Profile、Report資料 <視窗>
    
    - Missed chats
        - filter 控制項
            - Username
                * 輸入框
                * 預設文字：Username
            - Marketing
                * 下拉式選項
            - Login Time
                * 下拉式選項
                - 選擇custom period，展開時間選擇器，最久可以查詢到180天前的資料
            - IP
                * 輸入框
        - Search按鈕
            - 點擊後，使用設置的選項條件，頁面刷新 <API>
        - Export CSV按鈕
            - 點擊依頁面選擇的欄位匯出csv檔
        - Columns
            * 下拉式勾選項
            * 選擇後，下方表格依據篩選後顯示結果
        - Save按鈕
            - 保存顯示欄位 <API>
            * 保存成功提示文字：Save Success !
            * 保存失敗提示文字：Save Fail !
        -分析圖
            - Canvas
            - 資料顯示 <API>
            - 依據日期選擇區間顯示折線圖
                * 預設過去7天
            - 點擊折線圖日期 , 顯示當日錯過的聊天次數 , 下方依據點選日期顯示報表
        - table
            - 排序
            - 分頁
            - 顯示總筆數
            - 小計
            - 切換顯示筆數
                * 可選擇2、3、5、10
                * 預設顯示10筆
            - 表單資料顯示 <API>
            - Username
                - 點擊客戶名稱顯示Profile、Report資料 <視窗>
                    * 右側滑入視窗
            - View按鈕
                - 點擊顯示歷史聊天對話視窗、Profile、Report資料 <視窗>

    - Chat satisfaction
        - filter 控制項
            - Username
                * 輸入框
                * 預設文字：Username
            - Agent
                * 搜尋下拉式選項
                * 預設文字：Select agent
            - Chat satisfaction
                * 下拉式選項
            - Marketing
                * 下拉式選項
            - Login Time
                * 下拉式選項
                - 選擇custom period，展開時間選擇器，最久可以查詢到180天前的資料
            - IP
                * 輸入框
        - Search按鈕
            - 點擊後，使用設置的選項條件，頁面刷新 <API>
        - Export CSV按鈕
            - 點擊依頁面選擇的欄位匯出csv檔
        - Columns
            * 下拉式勾選項
            * 選擇後，下方表格依據篩選後顯示結果
        - Save按鈕
            - 保存顯示欄位 <API>
            * 保存成功提示文字：Save Success !
            * 保存失敗提示文字：Save Fail !
        -分析圖
            - 平均滿意度
                - Canvas
                - 資料顯示 <API>
            - 折線圖
                - Canvas
                - 資料顯示 <API>
                - 依據日期選擇區間顯示折線圖
                    * 預設過去7天
        - table
            - 排序
            - 分頁
            - 顯示總筆數
            - 小計
            - 切換顯示筆數
                * 可選擇2、3、5、10
                * 預設顯示10筆
            - 表單資料顯示 <API>
            - Username
                - 點擊客戶名稱顯示Profile、Report資料 <視窗>
                    * 右側滑入視窗
            - View按鈕
                - 點擊顯示歷史聊天對話視窗、Profile、Report資料 <視窗>


    - Chat surveys
        - filter 控制項
            - Marketing
                * 下拉式選項
            - Date
                * 下拉式選項
                - 選擇custom period，展開時間選擇器，因為有圖表呈現問題，故篩選可以查詢的區間範圍為30天
                * 最久可以查詢到180天前的資料(由今天往前推180天),區間範圍30天
                * 預設Last 7 days
            - Username
                * 輸入框
                * 預設文字：Username
            - Title
                * 下拉式選項
                - 顯示所有設定的聊天後問券名稱 <API>
                * 預設：空值
                * 提示文字：Title
            - 預設頁面
                - 預設頁面為空，依據篩選項顯示篩選後頁面，請參照設計檔？
        - Search按鈕
            - 點擊後，使用設置的選項條件，頁面刷新 <API>
        - Export CSV按鈕
            - 點擊依頁面選擇的欄位匯出csv檔
        -分析圖
            - 圓餅圖
                - Canvas
                - 資料顯示 <API>

    - 歷史聊天對話視窗
        - 聊天紀錄
            - 用戶名稱
            - 開始時間
            - 舊的對話紀錄 <API>
                - 對話
                    - 客服左側
                    - 客戶右側
                    - 頭像
                    - 時間
                    - 訊息內容
        - 資訊區塊
            - 切換顯示Profile、Report
            - 遊客身分說明
                - Profile資料僅顯示Username、Currency 、Channel Name
                - Report：顯示資料為空
            - Profile
                - Remark
                    - 資料顯示 <API>
                    - EDIT
                        - 編輯該筆資料 <視窗>
                        - 確認 <API>
                            - 更新列表 <API>
                        - 取消
                - General
                    - 資料顯示 <API>
                - Summary
                    - 資料顯示 <API>
                - Bank
                    - table
                        - 資料顯示 <API>
                        - EDIT
                            - 編輯該筆資料 <視窗>
                            - 確認 <API>
                                - 更新列表 <API>
                            - 取消
                - Balance
                    - 資料顯示 <API>
                - Technology
                    - 資料顯預設顯示10筆示 <API>
            - Report
                - Bet
                    - table
                        - 排序
                        - 分頁
                        - 顯示總筆數
                        - 小計
                        - 切換顯示筆數
                            * 可選擇2、3、5、10
                            * 預設顯示10筆
                        - 資料顯示 <API>
                        - View按鈕
                            - 開啟Report Detail
                    - Report Detail <視窗>
                        - table
                            - 排序
                            - 分頁
                            - 小計
                            - 顯示總筆數
                            - 資料顯示 <API>
                            - View按鈕
                                - 查看詳細資料，點擊另開分頁
                    - 分頁
                        - 資料顯示 <API>
                - Transfer
                    - Status
                        - 下拉式選單
                        * 包含All、Pending、Success、Fail
                    - table
                        - 排序
                        - 分頁
                        - 顯示總筆數
                        - 切換顯示筆數
                            * 可選擇2、3、5、10
                            * 預設顯示10筆
                        - 資料顯示 <API>
                        - Action按鈕
                            - 彈跳視窗 <視窗>
                            - ？
                - Deposit
                    - Status
                        - 下拉式選單
                        * 包含All、Pending、Approved、Disapproved
                    - table
                        - 排序
                        - 分頁
                        - 顯示總筆數
                        - 小計
                        - 切換顯示筆數
                            * 可選擇2、3、5、10
                            * 預設顯示10筆
                        - 資料顯示 <API>
                - Withdrawal
                    - Status
                        - 下拉式選單
                        * 包含Pending、On Hold、Rejected、Verified、Reverted、Disapproved、Processing、Approved
                    - table
                        - 排序
                        - 分頁
                        - 顯示總筆數
                        - 小計
                        - 切換顯示筆數
                            * 可選擇2、3、5、10
                            * 預設顯示10筆
                        - 資料顯示 <API>
                - Adjustment
                    - table
                        - 排序
                        - 分頁
                        - 顯示總筆數
                        - 切換顯示筆數
                            * 可選擇2、3、5、10
                            * 預設顯示10筆
                        - 資料顯示 <API>
                - Bonus
                    - Status
                        - 下拉式選單
                        * 包含All、Inactive、Active、Complete、Return to main、Suspend、Expired、Auto force serve、Manual force serve
                    - table
                        - 排序
                        - 分頁
                        - 顯示總筆數
                        - 小計
                        - 切換顯示筆數
                            * 可選擇2、3、5、10
                            * 預設顯示10筆
                        - 資料顯示 <API>
                        - Action
                            - 點擊解除流水限制
                        - View
                            - 點擊查看細項
                        - 細項
                            - ？

### Chats Settings

    - Channels
        - Website
            - 提供使用者程式碼 <API>
            - Copy code按鈕
                - 點擊複製程式碼
                - 複製成功提示文字：Copied  to Clipboard ! Now paste it to your  site's code.
        - Chat page
            - 提供聊天室連結 <API>
            - 提示文字如下：Share your chat page link so customers can easily contact your business wherever they are.
            - Copy Link按鈕
                - 點擊複製網頁連結
                * 複製成功，按鈕反綠
                - 提示文字：Copied!

    - Customization
        - 市場列表 <API>
            - 市場資訊區塊
                - Appearance
                    - 點擊設定聊天室外觀 <視窗>
                - Language
                    - Create
                        - 點擊新增的語言 <視窗>
                    - 點擊設定已新增聊天室語言 <視窗>
                - Chat assignment
                    - 點擊設定聊天室分配方式 <視窗>
                - Inactivity timeouts
                    - 點擊設定聊天室超時 <視窗>
                - Preferred language assignment
                    - 點擊設定喜好語言分配 <視窗>

        - Create
            * 各項目整合視窗 & 個別視窗
            - Ｍarket
                * 下拉式選項
                - 預設文字：Ｍarketing
            - Appearance
                - MAXIMIZED WINDOW
                    * 單選項目
                - MINIMIZED WINDOW
                    * 單選項目
                - Widget position
                    - Align to
                        * 下拉式選項
                    - Side spacing
                        * 數值選項
                        * Px限制0-100
                        * 超過紅字提示: Value should be between 0-100
                    - Bottom spacing
                        * 數值選項
                        * Px限制0-100
                        * 超過紅字提示: Value should be between 0-100
                - Pick your theme color
                    - 選擇自定義色，展開色碼選擇
                - Customer's bubble
                    - 點擊下拉式選單，顯示色碼
                - Customer's text
                    - 點擊下拉式選單，顯示色碼
                - Agent's bubble
                    - 點擊下拉式選單，顯示色碼
                - Agent's text
                    - 點擊下拉式選單，顯示色碼
                - Confirm
                    - 點擊即保存設定 <API>
                - Preview
                    - 點擊顯示預覽彈跳視窗
                - Cancel
                    - 關閉視窗
            - Language
                - Chat widget language
                    - 選擇聊天室語言
                    * 下拉式選單
                - Top bar
                    - 聊天室表頭文字設定
                    * 輸入框
                - Welcome message
                    - 進入聊天室 ,  用戶看到的訊息
                    * 輸入框
                - Message placeholder
                    - 回覆訊息中 , 系統提示文字
                    * 輸入框
                - Queued visitor info
                    - 排隊用戶顯示的訊息
                    * 輸入框
                - Confirm
                    - 點擊即保存設定 <API>
                - Preview
                    - 點擊顯示預覽彈跳視窗
                - Cancel
                    - 關閉視窗
            - Chat assignment
                - Auto assignment
                    * 單選項
                    - 問號
                        - 點擊顯示 : Chats are evenly distributed among agents with accepting chats status. When all agents hit their limit, new visitors are queued.
                - Manual selection
                    * 單選項
                    - 問號
                        - 點擊顯示提示文字 : All agents get notified about a customer waiting in the queue. Chat will be assigned to the first agent who picks it up.                
                - Confirm
                    - 點擊即保存設定 <API>
                - Cancel
                    - 關閉視窗
            - Inactivity timeouts
                - Transfer the visitor to another agent
                    - 輸入框
                    - 問號
                        - 點擊顯示：When the agent is not responding for   X    minutes, transfer the visitor to another agent.
                    - Status
                        - 狀態開關 , 預設關閉
                    - 僅設定Auto assignment 才會自動轉移給其他代理 , 選擇手動則不顯示此設定項
                - Close the chat
                    - 輸入框
                    - 問號
                        - 點擊顯示：When there are no new messages in the chat for  X minutes, close the chat.
                    - Status
                        - 預設關閉，若狀態開啟
                        - 沒有設定時間 , 則無法儲存
                - Confirm
                    - 點擊即保存設定 <API>
                - Cancel
                    - 關閉視窗
            - Preferred language  assignment
                - Status
                    - 狀態開關 , 預設關閉
                - Confirm
                    - 點擊即保存設定 <API>
                - Cancel
                    - 關閉視窗

    - Chat surveys ＆ forms
        - filter 控制項
            - Title
                * 下拉式選項
            - Type
                * 下拉式選項
            - Status
                * 下拉式選項
            - Marketing
                * 下拉式選項
                - 選擇Ｍarketing後 , 下方表格依據篩選後顯示結果
            - Created Time
                * 下拉式選項
                - 選擇custom period , 展開時間選擇器 , 最久可以查詢到180天前的資料(由今天往前推180天 , 超過180天以前的資料只能從資料庫撈資料)
        - Search按鈕
            - 點擊後，使用設置的選項條件，頁面刷新 <API>
        - Create
            - 點擊展開右側崁入視窗
        - table
            - 排序
            - 資料顯示 <API>
            - Status
                - 狀態顯示鈕 , 啟用或未啟用 <API>
            - Action
                - 點擊顯示修改彈跳視窗
            - Edit / Fill Out
                - 可編輯 / 不可編輯
        - Pre-chat survey / Update Pre-chat survey
            - Edit / Fill Out
                - 可編輯 / 不可編輯
            - Title
                * 輸入框
            - Type
                * 下拉式選單
            - Ｍarket
                * 下拉式選項
            - Name
                * 輸入框
                - 必填
            - E-mail
                * 輸入框
                - 必填
            - Language
                * 下拉式選單
            - Information
                * 輸入框
            - Qustion
                * 文字編輯器輸入框
                - Reqired
                    * 勾選項
                    - 是否為必填欄位
                - 垃圾桶icon
                    - 點擊刪除題目
                    - 需提示是否確認刪除
            - Choice list
                - Label
                    * 文字編輯器輸入框
                - Reqired
                    * 勾選項
                    - 是否為必填欄位
                - 垃圾桶icon
                    - 點擊刪除題目
                    - 需提示是否確認刪除
                - Choice#
                    * 輸入框
                - Add answer
                    - 新增單一選項欄位
                    - Choice#數字遞增
                    * 新增欄位無上限
                    - 垃圾桶icon
                        - 點擊刪除題目
                        - 需提示是否確認刪除
            - Dropdown
                - Label
                    * 文字編輯器輸入框
                - Reqired
                    * 勾選項
                    - 是否為必填欄位
                - 垃圾桶icon
                    - 點擊刪除題目
                    - 需提示是否確認刪除
                - Choice#
                    * 輸入框
                - Add answer
                    - 新增單一選項欄位
                    - Choice#數字遞增
                    * 新增欄位無上限
                    - 垃圾桶icon
                        - 點擊刪除題目
                        - 需提示是否確認刪除
            - Multiple Choice list
                - Label
                    * 文字編輯器輸入框
                - Reqired
                    * 勾選項
                    - 是否為必填欄位
                - 垃圾桶icon
                    - 點擊刪除題目
                    - 需提示是否確認刪除
                - Choice#
                    * 輸入框
                - Add answer
                    - 新增單一選項欄位
                    - Choice#數字遞增
                    * 新增欄位無上限
                    - 垃圾桶icon
                        - 點擊刪除題目
                        - 需提示是否確認刪除
            - Add element
                * 下拉式選項
                - 新增項目
            - Preview
                - 點擊顯示預覽彈跳視窗 <視窗>
                - Preview視窗
                    - 顯示全項目
                    - 。。。
            - Confirm
                - 點擊即保存設定 <API>
                - 頁面刷新 , 顯示新建項目 <API>
                - 增成功提示文字 : Insert Success!
            - Cancel
                - 點擊關閉
        - Post-chat survey / Update Post-chat survey
            - Edit / Fill Out
                - 可編輯 / 不可編輯
            - Title
                * 輸入框
            - Type
                * 下拉式選單
            - Ｍarket
                * 下拉式選項
            - Chat rating
                - Rating Lable
                    * 輸入框
                - comment Label
                    * 輸入框
            - Thank you message
                * 文字編輯器輸入框
            - Qustion
                * 文字編輯器輸入框
                - Reqired
                    * 勾選項
                    - 是否為必填欄位
                - 垃圾桶icon
                    - 點擊刪除題目
                    - 需提示是否確認刪除
            - Choice list
                - Label
                    * 文字編輯器輸入框
                - Reqired
                    * 勾選項
                    - 是否為必填欄位
                - 垃圾桶icon
                    - 點擊刪除題目
                    - 需提示是否確認刪除
                - Choice#
                    * 輸入框
                - Add answer
                    - 新增單一選項欄位
                    - Choice#數字遞增
                    * 新增欄位無上限
                    - 垃圾桶icon
                        - 點擊刪除題目
                        - 需提示是否確認刪除
            - Dropdown
                - Label
                    * 文字編輯器輸入框
                - Reqired
                    * 勾選項
                    - 是否為必填欄位
                - 垃圾桶icon
                    - 點擊刪除題目
                    - 需提示是否確認刪除
                - Choice#
                    * 輸入框
                - Add answer
                    - 新增單一選項欄位
                    - Choice#數字遞增
                    * 新增欄位無上限
                    - 垃圾桶icon
                        - 點擊刪除題目
                        - 需提示是否確認刪除
            - Multiple Choice list
                - Label
                    * 文字編輯器輸入框
                - Reqired
                    * 勾選項
                    - 是否為必填欄位
                - 垃圾桶icon
                    - 點擊刪除題目
                    - 需提示是否確認刪除
                - Choice#
                    * 輸入框
                - Add answer
                    - 新增單一選項欄位
                    - Choice#數字遞增
                    * 新增欄位無上限
                    - 垃圾桶icon
                        - 點擊刪除題目
                        - 需提示是否確認刪除
            - Rating
                - Rating Lable
                    * 輸入框
                - comment Label
                    * 輸入框
                - Reqired
                    * 勾選項
                    - 是否為必填欄位
            - Add element
                * 下拉式選項
                - 新增項目
            - Preview
                - 點擊顯示預覽彈跳視窗 <視窗>
                - Preview視窗
                    - 顯示全項目
                    - 。。。
            - Confirm
                - 點擊即保存設定 <API>
                - 頁面刷新 , 顯示新建項目 <API>
                - 增成功提示文字 : Update Success!
            - Cancel
                - 點擊關閉
        - 刪除視窗 ？
            - Cancel
                - 點擊關閉
            - Confirm
                - 點擊刪除資料 <API>
                - 頁面刷新 , 顯示更新資料 <API>
                - 增成功提示文字 : Update Success!
    - Canned responses
        - filter 控制項
            - Category
                * 輸入框
            - Marketing
                * 下拉式選項
                - 選擇Ｍarketing後 , 下方表格依據篩選後顯示結果
            - Created Time
                * 下拉式選項
                - 選擇custom period , 展開時間選擇器 , 最久可以查詢到180天前的資料(由今天往前推180天 , 超過180天以前的資料只能從資料庫撈資料)
            - Status
                * 下拉式選項
        - Search按鈕
            - 點擊後，使用設置的選項條件，頁面刷新 <API>
        - Create
            - 點擊展開右側崁入視窗
        - table
            - 排序
            - 資料顯示 <API>
            - Action
                - 點擊顯示修改彈跳視窗
        - Create
            - Ｍarket
                * 下拉式選單
            - Category
                * 輸入框
            - 輸入回覆的答案
                * 輸入框
                - 垃圾桶icon
                    - 點擊刪除文字
            - 輸入快捷鍵文字
                * 輸入框
                - “?”符號
                    - 滑鼠點過去顯示提示文字：To use a canned response during a chat, type in # and a shortcut. 提示客服使用快捷鍵須帶#符號
                - 垃圾桶icon
                    - 點擊刪除文字
            - Add
                - 點擊新增Canned response text…、Shortcut…欄位
            - Status
                - 點擊狀態為開啟 / 關閉
            - Confirm
                - 點擊即保存設定 <API>
                - 頁面刷新 , 顯示新建項目 <API>
                - 增成功提示文字 : Success!
            - Cancel
                - 關閉視窗
        - Update
            - Ｍarket
                * 下拉式選單
            - Category
                * 輸入框
            - 輸入回覆的答案
                * 輸入框
                - 垃圾桶icon
                    - 點擊刪除文字
            - 輸入快捷鍵文字
                * 輸入框
                - 垃圾桶icon
                    - 點擊刪除文字
            - Add
                - 點擊新增Canned response text…、Shortcut…欄位
            - Status
                - 點擊狀態為開啟 / 關閉
            - Confirm
                - 點擊即保存設定 <API>
                - 頁面刷新 , 顯示更新資料 <API>
                - 增成功提示文字 : Update Success!
            - Cancel
                - 關閉視窗

### System Settings

    - Role
        - filter 控制項
            - Name
                * 輸入框
            - Status
                * 下拉式選項
        - Search按鈕
            - 點擊後，使用設置的選項條件，頁面刷新 <API>
        - Create
            - 點擊展開右側崁入視窗
        - table
            - 排序
            - 分頁
            - 顯示總筆數
            - 切換顯示筆數
                * 可選擇2、3、5、10
                * 預設顯示10筆
            - 資料顯示 <API>
            - Action
                - 修改按鈕
                    - 點擊顯示修改彈跳視窗
                - 刪除
                    - 點擊顯示關閉彈跳視窗
        - Create <視窗>
            - Name
                * 輸入框
                - 輸入規則：4-20文字 , 包含英文/數字/英數 , 不得輸入符號
            - Status
                - 點擊狀態為Active / Inactive
            - Access Rights
                - 似乎是三維資料陣列
                - Check All
                    - 點擊勾選全部權限 ？
                - Expand
                    - 點擊展開所有細項
                - Close
                    - 點擊縮小至所有大項
            - Cancel
                - 點擊關閉
            - Confirm
                - 點擊即保存設定 <API>
                - 頁面刷新 , 顯示新建項目 <API>
                - 增成功提示文字 : Success!
        - Update <視窗>
            - Name
                * 輸入框
                - 輸入規則：4-20文字 , 包含英文/數字/英數 , 不得輸入符號
            - Status
                - 點擊狀態為Active / Inactive
            - Access Rights
                - 似乎是三維資料陣列
                - Check All
                    - 點擊勾選全部權限 ？
                - Expand
                    - 點擊展開所有細項
                - Close
                    - 點擊縮小至所有大項
            - Cancel
                - 點擊關閉
            - Confirm
                - 點擊即保存設定 <API>
                - 頁面刷新 , 顯示更新資料 <API>
                - 增成功提示文字 : Update Success!

    - Staff
       - filter 控制項
            - Username
                * 輸入框
            - Name
                * 輸入框
            - Role
                * 下拉式選項
            - Status
                * 下拉式選項
            - Marketing
                * 下拉式選項
                - 選擇Ｍarketing後 , 下方表格依據篩選後顯示結果
            - Language
                * 下拉式選項
        - Search按鈕
            - 點擊後，使用設置的選項條件，頁面刷新 <API>
        - Create
            - 點擊展開右側崁入視窗
        - table
            - 排序
            - 分頁
            - 顯示總筆數
            - 切換顯示筆數
                * 可選擇2、3、5、10
                * 預設顯示10筆
            - 資料顯示 <API>
            - Action
                - 修改按鈕
                    - 點擊顯示修改彈跳視窗
                - 刪除
                    - 點擊顯示關閉彈跳視窗
        - Create <視窗>
            - Username
                * 輸入框
                - 規則 : 支援6~12位英文、數字 , 不包含符號
            - Name
                * 輸入框
                - 規則 : 支援6~12位英文、數字 , 不包含符號
            - Password
                * 輸入框
                - 輸入限制 :  6~20位英文及數字 , 包含符號
            - Confirm Password
                * 輸入框
            - Role
                * 下拉式選單
            - Chats limit
                * 輸入框
            - Ｍarketing
                * 下拉式勾選項
                * 單選
            - Language
                * 下拉式勾選項
                * 可以複選
            - Status
                * 下拉式選單
            - Cancel
                - 關閉視窗
            - Confirm
                - 點擊即保存設定 <API>
                - 頁面刷新 , 顯示新建項目 <API>
                - 增成功提示文字 : Insert Success!
        - Update <視窗>
            - Username
                * 輸入框
                - 規則 : 支援6~12位英文、數字 , 不包含符號
            - Name
                * 輸入框
                - 規則 : 支援6~12位英文、數字 , 不包含符號
            - Password
                * 輸入框
                - 輸入限制 :  6~20位英文及數字 , 包含符號
            - Confirm Password
                * 輸入框
            - Role
                * 下拉式選單
            - Chats limit
                * 輸入框
            - Ｍarketing
                * 下拉式勾選項
                * 單選
            - Language
                * 下拉式勾選項
                * 可以複選
            - Status
                * 下拉式選單
            - Cancel
                - 關閉視窗
            - Confirm
                - 點擊即保存設定 <API>
                - 頁面刷新 , 顯示更新資料 <API>
                - 增成功提示文字 : Update Success!
        - 刪除視窗 <視窗>
            - Cancel
                - 點擊關閉
            - Confirm
                - 點擊刪除資料 <API>
                - 頁面刷新 , 顯示更新資料 <API>
                - 增成功提示文字 : Update Success!

    - Trusted domains
        - table
            - 排序
            - 分頁
            - 顯示總筆數
            - 切換顯示筆數
                * 可選擇2、3、5、10
                * 預設顯示10筆
            - 資料顯示 <API>
            - Action
                - 修改按鈕
                    - 點擊顯示修改彈跳視窗
                - 刪除
                    - 點擊顯示關閉彈跳視窗
        - Create <視窗>
            - Domain
                * 輸入框
            - Status
                - ON / OFF 切換紐
            - Cancel
                - 點擊關閉
            - Confirm
                - 點擊即保存設定 <API>
                - 頁面刷新 , 顯示新建項目 <API>
                - 增成功提示文字 : Insert Success!
        - Update <視窗>
            - Domain
                * 輸入框
                - 顯示反灰的Domain, 不能修改
            - Status
                - ON / OFF 切換紐
            - Cancel
                - 點擊關閉
            - Confirm
                - 點擊即保存設定 <API>
                - 頁面刷新 , 顯示更新後資料 <API>
                - 增成功提示文字 : Update Success!
        - 刪除視窗 <視窗>
            - Cancel
                - 點擊關閉
            - Confirm
                - 點擊刪除資料 <API>
                - 頁面刷新 , 刪除該項目 <API>
                - 增成功提示文字 : Update Success!
    - Banned Customers
        - todo
    - IP Whitelist
        - todo
