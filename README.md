# YouChang（友唱） -EmotionProject

友唱Emotion Project是基于[微软认知服务表情API](https://www.microsoft.com/cognitive-services/en-us/emotion-api)的实现友唱用户情感识别的代码样例。该样例包括以下Azure服务：
- Azure Linux VM
- Azure Storage
- Azure Cognitive Service: Emotion API
第三方的产品：
- [libcurl](https://curl.haxx.se/libcurl/c/libcurl.html)

该样例也可以作为在C语言环境下使用libcurl，实现调用微软认知服务REST API的样例。

## Emotion Project- 样例场景 ##

该样例业务场景是，使用微软认知服务的情感API，识别用户在唱歌过程中的情绪状态。具体技术架构如下：

*Figure 1. 友唱样例架构图*

![youchang Emotion Project Architecture](./YouChang01.PNG)


## Architecture ##
The Gump Come Smart Vending Machine solution architecture can be represented as follows:
- The Gump Come vending machine client will send its device status data to the Azure IoT Hub every 3 minutes. This data includes device status, goods channel status, and temperature. 
- Stream Analytics will transfer this data into three tables on Azure SQL Database, then Power BI will synch these table updates into the admin dashboard. 
