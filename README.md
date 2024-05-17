# unipapa 前台
https://www.unipapa.com/

![img](https://d1jjjfa1mlyr2v.cloudfront.net/u/2024-05-17-06-21-52_5f55708f41fd3b139dab8273cfdb5ed2.png)

nuxt 2.3.4

錯誤回報使用Sentry

css framework: tailwind

使用beanstalk做cicd

三方登入 google, line, fb

金流用tappay, 綠界, 街口支付, linepay

雖然是NUXT專案 但後來把大部分頁面的撈取資料都改成前端撈

而不是server撈取 為了減少server負擔跟增快速度

而商品頁還是保留用server撈 才會有meta資訊

#### unipapa 前台api專案

使用express 資料庫套件使用sequelize

---

# unipapa 後台

![img](https://d1jjjfa1mlyr2v.cloudfront.net/u/2024-05-17-06-22-03_4a6e89134a3109539f8a6e8c5d3088e6.png)

使用PHP 8.1 

Laravel 8.75

有實作權限管理, 分成管理員登入 廠商登入

曾經想要把會計的東西做進去 後來作罷

有串接發票系統

優惠碼, 促銷時段設定, 訂閱訂單每日檢查觸發付款

資料庫Mysql

css framework: bootstrap

js framework: vue2

---

# sheeper 前台

https://www.sheeper.com.tw/

![img](https://d1jjjfa1mlyr2v.cloudfront.net/u/2024-05-17-06-22-11_ee28e706191eeebc376e73f6c355470e.png)

single page application 使用vue3

css framework: tailwind

因為是spa 所以無法為不同的網址吐出不一樣的meta資訊

所以使用prerender 寫入資料庫

再使用nginx遇到fb或是twitter各種社群的要求時

撈資料庫吐出html而不是spa的html

寫入資料庫的html 使用nodejs的puppeteer給予網址就可以得到處理過的html

使用指令把build後的css跟js傳到s3 放到CDN讓速度變快

#### sheeper 前台 api專案

使用express 資料庫套件使用sequelize

---

# sheeper 後台

![img](https://d1jjjfa1mlyr2v.cloudfront.net/u/2024-05-17-06-22-18_1492d293c7eefa55acfce6e02f15ceef.png)

使用PHP 8.1

Laravel 8.75

資料庫Mysql

css framework: tailwind

js framework: vue2

---

# dr-ai

![img](https://d1jjjfa1mlyr2v.cloudfront.net/u/2024-05-17-06-22-34_494d61ff3f7147aa31396347f98645eb.png)


串接別人的api 類似聊天對話的網頁

single page application 使用vue3

css framework: tailwind

---

# stock

![img](https://d1jjjfa1mlyr2v.cloudfront.net/u/2024-05-17-06-22-43_a3df205c0af7179f1d53df7b5395d997.png)
![img](https://d1jjjfa1mlyr2v.cloudfront.net/u/2024-05-17-06-22-52_d8ebef4ee8c80e8499159d728c10464a.png)

自製股票系統 使用排程爬臺灣證券交易所的每日股票資料

然後列出簡易的表格跟畫圖

使用PHP 8.1 

Laravel 8.54

資料庫Mysql

---

# 雲端服務

用過GCP 但經驗不是很多

大多使用AWS 主要用ec2, rds, s3, beanstalk, route 53, cloudfront, load balance

曾經實作過code deploy, auto scaling, 透過指令更新

但後來就不使用了 cicd的經驗還算淺薄