# AWS IoT

官網連結：[https://aws.amazon.com/tw/iot/](https://aws.amazon.com/tw/iot/)

AWS IoT 是一種能夠將裝置連接至 AWS 服務和其他裝置、保護資料和互動安全、處理和對裝置資料採取動作，以及即使離線也能讓應用程式與裝置互動的平台。

![](https://m.media-amazon.com/images/G/01/DeveloperBlogs/AmazonDeveloperBlogs/legacy/AWS_IoT23._CB520207442_.png)

## 規則引擎（Rule Engine）

規則引擎可以將訊息路由到 AWS 終端節點，包含：

* AWS Lambda
* Amazon Kinesis
* Amazon S3
* Amazon Machine Learning
* Amazon DynamoDB
* Amazon CloudWatch
* Amazon Elasticsearch Service 搭配內建 Kibana 整合

使用 AWS Lambda、Amazon Kinesis 和 Amazon Simple Notification Service（SNS）可以存取外部終端節點。

## 裝置陰影（Device Shadow）

* 為每個裝置建立永久的虛擬版本，其中包含裝置的最新狀態，可讓應用程式或其他裝置讀取訊息並與裝置互動。
* 使用 Device Shadow 即使裝置離線，也能保留每個裝置的上次報告狀態及所需的未來狀態。
* 可以透過 API 或使用規則引擎來擷取裝置的上次報告狀態或設定所需的未來狀態。
* 應用程式不必考慮裝置的目前狀態即可設定裝置所需的未來狀態。
* AWS IoT 會比較所需未來狀態和上次報告狀態之間的差異，並命令裝置填補之間的差距。
* Device Shadow 可免費存放裝置的狀態多達一年。至少每年更新一次就能永久保留 Device Shadow，否則就會過期。

## AWS IoT Core

官網連結：[https://aws.amazon.com/tw/iot-core/](https://aws.amazon.com/tw/iot-core/)

AWS IoT Core 計算器：[Download Link](https://d1.awsstatic.com/IoT/assets/AWS_IoT_Core_Pricing_Calculator.0097ce19f649b854b9480f6330573f2e805ca6b7.xlsx)

