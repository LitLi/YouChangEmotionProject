# <YouChang>-EmotionProject

Microsoft teamed up with Gump Come, a provider of smart vending machines, to develop a way to monitor the working status of its machines and to get real-time information on replenishment needs. 
17
## Customer ##
[Gump Come](http://www.gumpcome.com/) is a leading AI innovation-oriented provider of smart vending machines and smart micro-supermarkets in China. These machines integrate the use of cameras, multi-touch, voice interaction, and big data analysis to realize new human-computer interaction patterns. 
 
## Pain point ##
To date, Gump Come has no solution that can monitor vending machine health status or get real-time information on whether a device is working. Any device needing attention usually requires two onsite visits—once to diagnose the issue and again to return with the component to fix the issue. All this adds to the cost of maintaining the machines.
The Gump Come goods manager must check on the selling status of the vending machines to see if they need replenishing. They want to develop an app for this. The goods manager will need training to learn to use the app. They want to get this information only through text or voice on the web app, and to reduce their cost of installing, learning, and updating the application. 
## Solution ##
1. Use Azure IoT Hub to collect data on supplies and device health for all vending machines and send to the uniform management platform for daily monitoring. This will help the staff to diagnose device issues online, which can save on maintenance costs and help realize predictive maintenance cost savings.
2. Based on Bot Framework and LUIS Services, build a vending machine management bot for an operator to check on vending machines and the status of their goods supply.

In this Smart Vending Machine solution, Gump Come will use the following Microsoft technologies: 
- Azure IoT Hub
- Stream Analytics
- Azure SQL Database
- Power BI
- Bot Framework

## Architecture ##
The Gump Come Smart Vending Machine solution architecture can be represented as follows:
- The Gump Come vending machine client will send its device status data to the Azure IoT Hub every 3 minutes. This data includes device status, goods channel status, and temperature. 
- Stream Analytics will transfer this data into three tables on Azure SQL Database, then Power BI will synch these table updates into the admin dashboard. 
