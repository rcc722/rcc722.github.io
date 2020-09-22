---
title: 小程序day1
---

#### 小程序基础 第一天

---

##### 一、微信开发的概述(能够描述出来)

###### 001 - 什么是微信开发

> 微信对外提供了例如：聊天、支付、分享、收藏、人工智能等功能，同时微信还对外开放了很多的接口与能力，
>
> 程序员基于这些功能和接口进行的开发，叫做微信开发

###### 002 - 为什么要学习微信开发

- 企业开发的需要
- 个人的发展以及技能的提升

课下阅读：[微信开发](https://baike.baidu.com/item/微信开发/1771495?fr=aladdin)

---

##### 二、了解微信开放平台(了解即可)

> 微信开发平台是微信对外提供**微信开放接口**的一个平台，这些开发出来的微信接口，供**第三方的网站**或**App**使用

###### 001 - 微信开放平台

平台登录地址：[微信开发平台](https://open.weixin.qq.com/)

###### 002 - 微信开放平台提供的能力

- 微信分享
- 微信支付
- 微信登录
- 微信收藏
- ……等等

###### 003 - 谁会使用微信开放平台

- 网站应用开发(第三方网站)
- 移动应用开发(例如第三方`App`)
- 第三方平台开发
- 公众帐号开发

###### 004 - 资质认证相关知识

- 只有通过 开发者资质认证后，才能使用开发平台提供的能力
- 个人名义无法申请资质认证，必须是公司或者一个团体才可以申请
- 只有企业类型的主体，才能申请资质认证

---

##### 三、微信公众平台(了解即可)

###### 001、微信公众平台

1.  微信公众平台

    是运营者通过公众号这个媒介，为微信用户提供咨询和服务的平台

2.  微信公众平台开发

    指基于微信公众号进行的业务开发

3.  [平台登录地址](https://mp.weixin.qq.com/)

###### 002、微信公众平台的账号分类

> 微信公众平台的账号统称为公众号

![](./images/mp.png)

###### 003、如何选择自己的公众号类型

- 订阅号 -- 简单的发送消息，达到宣传效果，建议选择订阅号
- 服务号 -- 想用公众号获得更多的功能、提供更多的服务，例如开通微信支付，建议选择服务号
- 小程序 -- 想提供类似于手机 `App` 的服务体验，建议选择小程序
- 企业微信(原企业号) -- 想用来管理内部企业员工、团队，对内使用，进行以选择企业微信(原企业号)

---

##### 四、开放平台和公众平台的区别(理解记忆)

###### 001、开放平台

- 是微信对外开放 `API` 接口的平台
- 开放的 `API` 接口，供第三方网站和 `App` 调用
- 后端程序员是开放平台开发的主力军

###### 002、公众平台

- 是基于微信公众号，为微信用户提供服务的平台
- 所用公众号，都属于微信内开发
- 前端程序员是公众平台开发的主力军

---

##### 五、认识小程序

###### 001、什么是小程序

> 微信小程序是一种全新的连接用户和服务的媒介，它可以在微信内被便捷地获取和传播，同时具有出色的使用体验

- 小程序的特点： 体积小、方便获取与传播
- 小程序的理念： 用完即走

###### 002、 小程序出现的目的

- 拦截用户流量入口，用户的大多数应用需求，都可以才能够微信小程序中得到满足

###### 003、 小程序和订阅号、服务号的区别

- 发布时间不同
- 2017-07 公众平台发布
- 2017-01 小程序发布
- 入口方式不同
- 订阅号、服务号是作为微信联系人存在的
- 小程序有自己的独立入口
- 体验效果不同
- 订阅号、服务号体验差、无法提供类似于 `App` 的体验
- 小程序模拟了手机 `App` 的体验，更人性化

###### 004、小程序适合的业务场景

- 适合做用完即走的应用
  - 例如： 点外卖、打车、代驾、共享单车等
- 不适合做重度依赖的应用
- 例如：大型手机游戏类、音乐播放器等

###### 005、小程序和传统手机 `App` 的区别

- 开发原理不同
- `App` ： 基于手机操作系统提供的 `API` 进行开发
- 小程序：基于微信提供的 `API` 进行开发
- 运行方式不同
- `App`： 直接安装并运行在手机操作系统之上
- 小程序：必须基于手机微信才能安装和运行

![小程序和传统手机 `App` 的区别](./images/mina.png)

---

##### 六、小程序中的组件

> 组件是视图层的基本组成单位，自带一些功能与微信风格一致的样式

1.  初始组件

一个组件通常包括**开始标签** 和 **结束标签**，**属性** 用来修饰这个组件，**内容**在两个标签之间

**注意：** 所有 **组件名称** 与 **属性名称** 都是小写

```javasc
<button type="primary">primary</button>
```

![primary](./images/primary.png)

2.  推荐阅读

- [组件介绍](https://developers.weixin.qq.com/miniprogram/dev/framework/view/component.html)
- [组件文档](https://developers.weixin.qq.com/miniprogram/dev/component)

---

##### 七、小程序中的 `API`

###### 001 - `API` 的概念

1. `API` 应用程序编程接口，是一些预先定义的函数，目的是提供应用程序与开发人员基于某软件或硬件得以访问一组例程的能力
2. 小程序开发框架提供丰富的微信原生 `API`，可以方便的调起微信提供的能力，如获取用户信息，本地存储，支付功能等。

###### 002 - `API` 的三种分类

1.  事件监听 `API`

- 以 `on` 开头的 `API` 用来监听某个事件是否触发

2.  同步 `API`

- 以 `Sync` 结尾的 `API` 都是同步 `API`

3.  异步 `API`

- 通常需要指定回调函数接受调用的结果
- 小程序中，大多数的 `API` 都是异步 `API`

4.  推荐阅读

- [API 介绍](https://developers.weixin.qq.com/miniprogram/dev/framework/app-service/api.html#API)
- [API 文档](https://developers.weixin.qq.com/miniprogram/dev/api/)

---

##### 八、组件和 `API` 的异同点

1.  相同点

- 组件和 `API` 都是微信官方给提供的
- 组件和 `API` 的目的，都是为了方便小程序的快速开发

2.  不同点

- 组件以 `UI` 结构布局为主， 一般不需要处理业务逻辑
- `API` 以纯业务逻辑为主，一般没有对应的 `UI` 结构

---

##### 九、注册小程序账号

1.  参考网址

- [小程序接入指南](https://developers.weixin.qq.com/miniprogram/introduction/#注册小程序帐号)
- [微信小程序开发注册](https://mp.weixin.qq.com/cgi-bin/wx?token=&lang=zh_CN)
- [小程序申请账号](https://developers.weixin.qq.com/miniprogram/dev/framework/quickstart/getstart.html#申请帐号)

---

##### 十、小程序基本信息设置

1.  登录小程序账号 --> 设置 --> 基本设置

---

##### 十一、小程序账号的开发设置

1.  登录小程序账号 --> 开发 --> 开发设置
2.  既可以查看到在实际开发中需要获取以及设置的开发者 ID 以及服务器域名

---

##### 十二、小程序账号的成员管理

###### 001 - 成员管理的概念

1.  一个团队进行小程序开发，那么团队成员的身份管理是很有必要的
2.  管理员可在小程序管理后台统一管理项目成员、设置项目成员的权限

###### 002 - 权限说明

1.  运营者权限

- 管理、推广、设置等模块权限，可使用体验版小程序

2.  开发者权限

- 开发模块权限，可使用体验版小程序、开发者工具（`IDE`）

3.  数据分析者(基础分析)

- 统计模块权限，可使用体验版小程序

###### 003 - 添加方式

1.  登录小程序账号 --> 管理 --> 成员管理 -- 项目成员 -- 点击向下的箭头
2.  推荐阅读：[小程序成员管理](http://kf.qq.com/faq/170302zeQryI170302beuEVn.html)

![添加成员的方式](./images/person.png)

##### ![](./images/confirm.png)

---

##### 十三、微信开发者工具

[开发者工具下载地址](https://developers.weixin.qq.com/miniprogram/dev/devtools/download.html)

---

##### 十四、创建小程序项目

1.  打开小程序开发者工具，用微信扫码登录开发者工具
2.  点击左侧菜单中的小程序选项
3.  点击+号新建小程序项目
4.  填写项目名称
5.  选择项目存放路径（必须选择空目录）
6.  填写 `AppID`
7.  点击新建按钮

![](./images/newproject.png)

##### 十五、小程序预览

> 作用：通过预览功能，可以在真机环境下，快速查看小程序的实际效果

1.  点击 工具栏 --> 预览 即可弹出预览窗口
2.  预览方式：扫描二维码预览、自动预览

![小程序预览](./images/ma.png)

##### 十六、开发者工具主界面功能

1.  开发者工具主界面，从上到下，从左到右，分别为五大部分：

- 菜单栏
- 工具栏
- 模拟器
- 编辑器
- 调试器

![开发者工具主界面功能](./images/jiemian.png)