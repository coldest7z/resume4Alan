# Resume

## Contact

- Email：coldest7@foxmail.com
- Telegram：alanzhou

## Personal Information
 - Alan Zhou/1998
 - Changsha University
 - Years of working：5 years
 - Position Desired：Java Developer
   
## Skill Inventory
The following are the skills I have mastered：
- Language：Java/JavaScript
- Web Framework：Spring/SpringMVC/SpringBoot/SpringCloud/Mybatis/MybatisPlus
- Middleware：Redis/RocketMQ/RabbitMQ/Nginx
- Database：MySQL/OracleSQL/SQLServer
- Tools：SVN/Git/IDEA/VSCode/Navicat/Xshell/VirtualBox/OpenVPN/Postman/SoapUI

## Work Experience

### Telework (2022-01 ~ now)

#### The Financial System

**Project Description:** This project is outsourced to our team by Shenzhen Dashao Medical Health Technology Co., LTD., and the integration of industry and finance is a financial project of insurance channel business.

**Project Module:**

- ETL
  - This module is used to load the insurance order, business order, Wechat bill, and other related order data from other systems into the business finance system for account checking through export - conversion - cleaning
- Reconciliation
  - Design a general reconciliation model, check the business data in pairs, and monitor whether the business process is complete and the data is accurate.
- Settlement
  - Design general settlement process, and assist business personnel to settle with external suppliers according to the data completed by account reconciliation.
- Pay
  - Assist financial personnel in payment and collection of settlement and clearing data. (Direct connection between banks and enterprises)
- Accounting
  - Assist the financial personnel to handle the payment and payment data. (Docking Kingdee system)

### China Broadnet (2020-07 ~ 2022-01)

#### CPS

**Project Description:**China Broadnet and Television Snail TV internal platform system, responsible for the coordination and interaction of major systems.

**CPS Management System:**

- System management

- Configuration management

- Error retransmission

- User management

- Channel management

- SKU configuration

- Commodity management

- Product management

- Rights management

- Strategic management

- The order management

- Payment records

**CPS System:**

- Orders module
  - This module is responsible for connecting the business order information of each channel system and has the payment function
- Channels of distribution
  - After the user pays, it needs to be distributed to each channel provider system according to the configured SKU and receive the callback information to transfer to the order module
- Check module
  - On day T+1, the bill information of the payment platform was retrieved through FTP for reconciliation

### Hunan Star Shining Technology (2018-02 ~ 2020-07)

#### Finger Mall

**Project Description: **Fingerspelling is a new type of e-commerce project. Including Android APP, WeChat small program, administrator background, shop administrator background, provincial and municipal generation management background, docking WeChat small program payment, APP WeChat pays, and Alipay pays. The project adopts a micro-service architecture, with a total of 12 services, which will be detailed below. Mainly contains the core function for the group, for example, 100 users to spell a certain level of commodities, 97 users will not spell commodities, and 3 users will spell commodities; The system will give cash back to the 97 users who have not put up the goods, and the users who are putting up the goods can take away the goods, or they can choose to sell the goods on behalf of the users, which means that the system directly buys the users' goods and gives the users cash back.

**Project Service:**

- Customer service
  - Main functions for user registration landing: user registration must need an inviter, the system needs to maintain relationships, invite the number directly, the number of teams, according to the user to invite new users to judge the level, when reaching a certain level, the people who were invited as long as the spelling group did not spell goods, inviter according to level can obtain the corresponding money. This function uses asynchronous relationship maintenance, the main difficulty is the infinitely complex relationship tree between users (query and modify related performance issues), which has achieved the maximum registration performance
- System services
  - All levels of administrators management background, provincial and municipal generation management background, management of stores, audit of the user registered stores
- Goods and services
  - To search commodities, Canal+Logstash imported commodities in the database into Elasticsearch in real-time and used Elasticsearch to search
- Order service
  - Create an order, and modify the order. When users click the group, they will be added to the queue. 100 person will be taken out from the queue each time, and 3 people will be selected randomly to win the prize. User information, group information, and commodity information will be added to the MQ queue. The ordered service listens for MQ messages and generates orders asynchronously
- Routing gateway
  - All request entries, all service request addresses unified
- Separate accounting services
  - The user records the details related to the user's money, and as long as the money-related operations are involved, sends a message to MQ. This service will listen to the MQ message and save the information related to the user's money to Elasticsearch
- Details of the service
  - The user records the details related to the user's money, and as long as the money-related operations are involved, sends a message to MQ. This service will listen to the MQ message and save the information related to the user's money to Elasticsearch
- Message service
  - The system sends messages to all users and a certain user, such as the user group wins the lottery, the system upgrade announcement, and so on
- The store service
  - Store manager backstage, upload goods, store query store amount related details, etc
- Integral services
  - Users watch ads daily and can convert points to a balance, which can be withdrawn directly

- Spell group service
  - Users participate in the group entry, regular group formation, random winning and not winning users, user information, commodity information, and group information sent to the queue
- Video red envelope service
  - Upload the video, and set the red envelope information, the system will automatically create red envelopes at 12 o 'clock every day. Grab the red envelope, did not grab the red envelope back and so on

