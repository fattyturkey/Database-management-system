# Database-management-system

# 1.数据库系统和查询
1.数据库管理系统 Database Management System  (DBMS
是一种操纵和管理数据库的软件，由一套复杂组件协同工作，用于建立、使用和维护数据库。 
最重要的功能就是通过DB engine操作数据库里的数据

2.数据库引擎 Database engine
是用于存储、处理和保护数据的核心组件。由编程语言对Database Engine下达命令。常见的语言：SQL. 

3.结构化查询语言 Structured Query Language  (SQL
是一种数据库查询和程序设计语言，用于存取数据以及查询、更新和管理关系数据库系统。SQL有国际标准，
但各厂商在标准基础上额外添加了一些自己独特的功能，不同厂商的SQL会有些许不同。就比如微软的
SQL Server用的是T-SQL（T指Transact）。

4.客户端client/服务器server 软件架构：C/S架构
运行着的数据库管理系统叫做服务器。
C/S架构这种架构的软件有服务器和客户端，服务器负责数据的管理，客户端来完成与用户的交互任务.

5.图形用户界面 Graphical User Interface (GUI
采用图形方式显示的计算机操作用户界面。 
为了让用户能够以可视化的形式与DBMS交互，基本各个厂商都有自己配套的带有图形用户界面的客户端程序
SQL server的图形用户界面是Sql server management studio.(SSMS)
MySQL的客户端是MySQL Workbench.

6.用户怎样操作数据库：| 用户 --操作--> Client（SSMS） --指示--> Server（SQL Server） --查询--> 数据库 | 
准则：无论成功失败都要给用户一个反馈※※※※※※※
   
   
SQL Server是一个产品的名字   
![image](https://github.com/fattyturkey/Database-management-system/blob/main/IMG_0942.JPG)




7.数据库（Database）是按照数据结构来存储、组织和管理数据的仓库。是一个储存在计算机内的，
有组织，统一管理的大量数据的集合。Database由DatabaseEngine管理。

我们下载学习用的数据库是 OLTP（online transactional processing）線上交易處理是指透過資訊系統、電腦網路及資料庫，以線上交易的方式處理一般即時性的作業資料，还有OLAP(online analytical processing)data warehouse線上分析處理
OLAP通常與OLTP（線上交易處理）形成對比，OLTP的特點是查詢的複雜性要小得多，而且查詢量要大得多，以處理事務，而不是用於商業智慧型或報告。OLAP系統主要針對讀取進行最佳化，而OLTP得能處理各種查詢（讀取、插入、更新和刪除RCUD）。

数据库的类别：关系型数据库（Relational Database）和非关系型数据库。 
RelationalDatabase受到预设关系的约束。常常使用在对数据完整性，正确性要求比较高的应用上。Ex: 银行；Market.

文档型数据库（Document Database）：用作管理文档（记录）。在RelationalDatabase中，信息被分割成离散的数据段。
而在DocumentDatabase中，文档是处理信息的基本单位。一个文档可以很长，很复杂，也可以无结构，就像文档一样。
DocumentDatabase常常应用于Bigdata的存储和处理。Ex: Ads.（data不在于完整，而在于全收录，包括错误

我们正在学习的数据库是一种Ralational Database。SQL Server主要用于管理 Ralational Database

8.对数据进行ETL（Extract-Transform-Load）是一个 数据工程师 经常干的事。Extract：抽取数据；Transform：整理，变型；
Load装载，将数据包装给下游的数据分析师、数据科学家 

9.查询query
也被称为查或访问数据库。对数据库查询（Query）也指访问数据库。也就是通过客户端向DBMS问询数据库中的数据。
查询这一行动包含了四个行为，分别是：增、删、查、改，其中只有“查”不对文件做出改动。在英文中这四个行为被称作
（CRUD）C: Create[增]；R: Read[查]；U: Update[改]；D: Delete[删]。

# 2.查询
在SSMS中，对某一数据库新建查询，需在左侧图表中选中数据库，或在查询中使用use语句。
![image](https://github.com/fattyturkey/Database-management-system/blob/main/IMG_0667_%E5%89%AF%E6%9C%AC.png)
