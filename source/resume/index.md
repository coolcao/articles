---
title: resume
date: 2016-10-18 11:27:10
comments: false
---

## 曹洪升

nodejs工程师 | 电话：18500215563 | 邮箱：<a href="mailto:me@coolcao.com">me@coolcao.com</a> | 微信：434524099

个人博客：[coolcao.com](http://coolcao.com) | github：[github.com/coolcao](https://github.com/coolcao) | 掘金ID：[coolcao](https://gold.xitu.io/user/58115de20ce4630031a13d21)
## 教育
**2013**年毕业于**山东财经大学**，**信息管理与信息系统**专业,**本科**，目前已工作**3年半**

## 工作经历
|公司|职位|时间|主要职责|
|----|----|----|----|
| 乐视网		|nodejs工程师		|2016.06~至今|开发乐视边看边买互动后台系统|
|北京自在科技	|nodejs工程师		|2014.06~2016.06|API后台开发，官网重构，后台服务解耦|
|天融信		|Java工程师			|2013.07~2014.06|后台管理系统开发|

## 技术栈
* 熟练使用**nodejs，es6，express/koa2**构建web服务
* 熟悉 **mongodb**，**MySql**
* **docker容器技术,持续集成**
* 熟悉基本的**数据结构与算法**
* 了解并应用前端（html+css）技术构建web应用，熟练**angular,gulp,bootstrap**等构建SPA应用
* 熟悉 **linux,mac**工作环境

## 自我描述
目前重点在nodejs后台及前端开发方向，研究前后端分离方向。
前端发展很快，切记内功修炼，不可浮躁。

## 项目经验

##### 乐视边看边买后台	| 独立开发	|	2016.06~至今
* 边看边买后台系统管理广告引擎系统需要的广告业务数据。引擎提供给前端（PC，移动端，TV）的广告数据，由本系统管理。
* 负责功能模块：
	* 商品管理,对接阿里百川商品库以及乐视商城商品库商品数据，统一格式存入MongoDB
	* 广告模板管理，采用JSON动态指定模板格式及参数
	* 广告位管理，视频打点生成广告位以及对接智能识别系统获取广告位信息，统一入库MongoDB
	* 订单管理，提供运营人员选择商品，模板，广告位，广告等创建订单功能，订单冲突检测，会员定向，地域定向冲突检测功能
	* 权限角色管理，采用`用户-角色-权限`模型
* 技术方案：
 	* nodejs+angularjs前后端分离方案
 	* **nodejs+express**做后台rest接口，**PM2**管理node服务。
 	* 数据库**mysql + mongodb**
 	* 前端**angular+bootstrap**

##### 消息服务 | 设计与实现 | 2016.02～016.05
* API后台微服务化实践，将后台涉及到消息的业务拆分成一个单独的服务，docker部署
* 功能点
	* 采用MongoDB的固定集合实现发布订阅模式
	* API后台将消息发布到Mongo固定集合，消息服务订阅消息，并调用第三方服务（短信，推送，邮件）发送消息
	* 失败重试机制，如果消息发送失败，重试3次
	* 多台订阅服务路由机制，计算hash(uid)动态分配消息发送服务
	* 消息发送日志存储入库
* 技术方案
	* nodejs+es6编写发布订阅服务模块
	* mongodb固定集合实现发布订阅队列
	* postgresql存储消息发送记录日志

##### 自在科技官网 | 独立开发 | 2015.10～016.01
* 自在科技官网重写，前端项目
* nodejs+express+swig+bootstrap搭建基本web框架
* es6+less+gulp+nodemon搭建前端自动化构建服务
* 自在博客，多语言支持（i18n）以及其他静态页面展示
* docker+jenkins自动化部署运维

##### 自在科技运营后台 | 开发 | 2014.10~2015.09
* 为公司运营人员提供：
	* 用户信息查询功能
	* Nut贴片信息查询功能
	* 官网博客，招聘信息，FAQ等动态更新信息管理功能
* 技术方案
	* 采用前后端分离架构
	* nodejs+express后台rest服务接口
	* angularjs开发前台SPA应用
	* gulp+nodemon+browser-asyc搭建自动化开发环境

##### APP后台REST接口 | 开发/维护 | 2014.06～015.08
* Nut app后台rest接口开发
* 接口服务：spring+spring-boot
* 数据库：mysql+mybatis
