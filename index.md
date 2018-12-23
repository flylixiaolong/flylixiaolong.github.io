***
## 联系方式

- 手机：18616210489
- Email：fly_lxl@foxmail.com
- 微信号：18616210489 （C_Geek)

***
## 个人信息

 - 李小龙/男/1992 
 - 本科/中国石油大学(华东)/计算机科学与技术 
 - 工作年限：3年
 - 在线简历GitPages：[https://flylixiaolong.github.io](https://flylixiaolong.github.io)
 - Github：[https://github.com/flylixiaolong](https://github.com/flylixiaolong)
 - 期望职位：后端开发工程师
 - 熟练掌握：Python/Nodejs/Go
 - 期望城市：上海

---
## 工作经历

###  1. 店达商城：全栈工程师【偏后端】（ 2017年12月 ~ 至今 ）


###### 主要技术

nodejs, express, mysql, rabbitmq, redis, hprose(RPC), elk, ansible, html/css

###### 店达商城后端系统整合/单点登录项目
主要负责店达商城后端系统的合并和裁剪，合并/裁剪掉了部分可有可无的系统服务。实现已有的后端管理系统的S单点登录SSO功能(基于主域名cookie/session共享原理)，完成了12个业务管理系统的单点登录。兼容不同框架(express/koa)以及不同的项目架构(前后端分离与不分离项目)


###### 优惠分摊项目 
已有的订单逻辑不能满足财务对账的功能，并且出现退货时，优惠金额不算在订单金额内，造成一定的业务亏损。对已有的订单系统进行改造，完成从RPC到HTTP API的迁移工作。对已有的退货逻辑进行改造，按照优惠分摊后的SKU金额进行退货。

###### 猪行侠(配送APP)后端重构

配送系统和订单系统使用MQ消息同步订单状态，MQ/DB和业务系统共用一套HAproxy，由于对amqplib包使用不当，以及运维操作上的问题(重启或网络故障)导致系统间的通知消息偶尔会发生丢失的情况，查明原因后由运维将基础服务和业务系统的HAproxy分离，同时重构发送MQ消息的底层代码，采用ConfirmChannel进行消息发送，确保消息发送至MQ server。重构后该部分代码精简掉1/2。


###### 其他项目
- 商城库存管理系统优化（QOA系统）
- 客服系统开发和维护
- 仓库运输开发和维护

---
### 2. 明码生物：Python后端工程师（ 2016年4月 ~ 2017年9月 ）

###### 主要技术

python, django, celery, mysql, rabbitmq, redis, docker/docker-compose, jenkins, nginx, uwsgi, angular

###### LIMS-ext项目 / 报告系统项目
对接实验室信息管理系统(LIMS)和CSA系统，实现部分分析流程的自动化，并根据分析结果生产成PDF报告。负责实现从html到pdf的自动转换，根据分析结果生成对应的pdf报告。Django项目。部署：nginx + uwsgi + supervisor + django


###### Jenkins持续集成
实现项目的持续集成，打通Gitlab和Jenkins，根据不同的git分支或tag进行部署，测试环境按照开发分支每次提交即构建并执行单元测试和覆盖度测试，完成后发送结果邮件；预发布环境根据新增预发布分支进行自动构建；生产环境根据最新tag进行构建(手动触发)。实现方式：jenkins git plugin +
gitlab webhook + shell + docker + docker-compose


###### selenium+chromedriver的自动化测试
采用selenium+chromedriver编写LIMS系统的自动化测试脚本，每次发布系统前执行测试脚本，减轻人工负担。

###### 其它工作内容
- selenium+phantomjs爬虫
- airflow 工作流调度
- django和ldap集成

---

### 3. 中科院通用芯片与基础软件研究中心：软件工程师 （ 2015年7月 ~ 2016年4月 ）

###### 主要技术

linux, vim, python, c/c++, gcc, shell, gdb, makefile

###### Linux系统性能自动化测试项目
编写自动化脚本，运行Benchmark,  并对Benchmark运行结果进行提取，生成性能测试的PDF报告。可以对不同的两个系统的测试结果生产性能对比报告，并以图表形式展示差异。报告生成采用reportlab。


###### ICC/GCC下lbench位操作性能差异分析
用不同的编译器icc/gcc编译lbench后，发现在统一系统下lbench运行结果，位操作速度icc编译后的版本要比gcc版本快两个数量级。对此裁剪lbench代码，写测试代码，并对代码进行反汇编分析性能差异的具体原因。

###### gcc编译参数调优
使用OpenTuner(python package)进行编译参数调优，OpenTuner会记录每次进行编译的gcc参数和性能评估的结果，并采用迭代算法找到最优编译参数。

###### 其他项目
- linux文件系统分析

---
## 开源项目

 - [mq-reconnect](https://github.com/flylixiaolong/MQ-Reconnect#readme): 对amqplib的简单封装，实现断线重连机制，默认采用ConfirmChannel并提供更简单的使用接口

***
## 主要技能

- 后端开发：python, nodejs, django, express
- 前端开发：HTML, CSS，了解Vue, Angular,webpack
- 数据库：mysql, redis
- 消息队列：rabbitmq
- 版本控制：git, svn
- 代码调试：pdb, gdb
- 文本编辑：vim
- 运维工具：ansible, elk
- Python package: celery, sqlalchemy, scrapy, airflow, selenium, requests
- NPM package: request,  async,  sequelize,  lodash,  moment,  amqplib 

***
## 阅读书籍

- C程序设计语言【C Programming Language】
- C++ Prime
- 深入理解Linux内核【Understanding the Linux Kernel】
- 高性能Mysql
- Spark快速大数据分析
- Redis实战
- Unix环境高级编程【Advancd Programing in the Unix Environment】
- Python学习手册【Python Learning】
- Python CookBook
- Go程序设计语言【The Go Programming Language】
- Go语言实战【Go in Action】
- Building Applications on Mesos【用Mesos框架构建分布式应用】
