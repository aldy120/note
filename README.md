# 無伺服器架構 (serverless architecture) 
- John Chang (講者)
- Lambda
- API Gateway
- DynamoDB

# 優點
- 讓工程師可以更專注在程式碼，而不是伺服器的維護及建置。
- 關於伺服器方面，就交給Amazon維護，達到專業分工。
- 用多少資源付多少錢，也不用因為閒置資源而煩惱。

![img ](http://i.imgur.com/z2DKU3e.gif)
# Lambda
- 把伺服器藏起來，讓使用者不用花心思設定調整
- 可直接利用雲端工具寫程式
- 也可包成 zip 後上傳
- 也可以直接從 S3 匯入
- 支援多種程式碼(最近新增 python 3.6)
- 與 AWS 各項服務整合良好
- 費用與使用的時間與使用的儲存空間相關

# API gateway
- 使用模擬(mock)整合
- 可連接 Amazon Cognito，免去處理使用者登入相關問題

# DynamoDB
- 一種 NoSQL 資料庫
- 速度極快，適合即時串流服務
- 具可延展性，可隨時擴充資料庫大小
- 免擔心資料庫硬體細節

![img](http://imgur.com/Y8WM4qg.png)

# 觀眾提問
- 如何將 PHP + MySQL 上原有的服務直接轉移到 serverless 架構?
  - 產品若已上線，這麼做的風險太大
  - 開發新功能的時候可以嘗試做在 serverless 上面
  - 很多服務都有驗證使用者之類的工作，可以搬到
- 如何解決資安問題
  - 可以設定安全群組
  - 同樣可以進行 SA 及 QA
