title: Rainbow
---
![Rainbow 架构](.\images\rainbow-architecture.png)

## 技术架构

### AMD
AMD 全称是Asynchronous Module Definition，即异步模块加载机制。AMD 规范是JavaScript开发的一次重要尝试，它以简单而优雅的方式统一了JavaScript的模块定义和加载机制，并迅速得到很多框架的认可和采纳。这对开发人员来说是一个好消息，通过AMD我们降低了学习和使用各种框架的门槛，能够以一种统一的方式去定义和使用模块，提高开发效率，降低了应用维护成本。

### Framework
采用 SPA（单页 Web 应用框架）以 Ajax 为核心的服务请求模式，利用 RequireJS 基于 AMD 规范进行模块化开发和依赖管理，使用 jQuery 作为 DOM 操作类库，使用 Backbone 作为前端 MVC 框架，结合 Bootstrap 构建前端 UI 组件形成根据服务 API 动态渲染交互视图的 Web App 框架。


## API
以 JSON / JSONP 的方式与服务端引擎 API 发起请求并异步响应返回数据接口。

## 浏览器

### 桌面（Desktop）

IE 10+ 、 Chrome、Firefox、Safari

### 移动端（Mobile）

iOS、Android、Windows Phone