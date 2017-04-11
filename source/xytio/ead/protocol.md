title: 协议架构
---
![协议架构](.\images\protocol-architecture.png)

EAD 平台完全面向 Restful 风格的 API 进行设计开发，实现服务端与客户端的完全分离，采用目前业界最广泛应用的无状态 HTTP/HTTPS 协议为 Rainbow、移动客户端、第三方应用等各种形式的客户端提供数据服务。

### HTTP / HTTPS

超文本传输协议（英文：HyperText Transfer Protocol，缩写：HTTP ）是互联网上应用最为广泛的一种网络协议。设计 HTTP 最初的目的是为了提供一种发布和接收HTML页面的方法。通过 HTTP 或者 HTTPS 协议请求的资源由统一资源标识符（ Uniform Resource Identifiers，URI ）来标识。EAD 完全依托于 HTTP 协议进行服务的提供和访问。

### Restful

具象状态传输，REST 通常基于使用 HTTP，URI，和 JSON、XML 以及 HTML 这些现有的广泛流行的协议和标准。资源是由URI来指定。对资源的操作包括获取、创建、修改和删除资源，操作对应 HTTP 协议提供的 GET、POST、PUT 和 DELETE 方法。通过操作资源的表现形式来操作资源。资源的表现形式则是 JSON、XML 或者 HTML，取决于读者是机器还是人，是消费 Web 服务的客户软件还是 Web 浏览器。在目前 EAD 的架构体系中，资源的主要表现形式为 JSON 对象。

### Rest RPC

EAD 允许其它第三方程序使用 Rest RPC 方式以用户身份进行所有 API 的远程访问和操作。

### Websocket

WebSocket 是 HTML5 开始提供的一种在单个 TCP 连接上进行全双工通讯的协议。WebSocket 通讯协议于 2011 年被IETF定为标准 RFC 6455，WebSocketAPI 被 W3C 定为标准。在现代浏览器和主流移动设备中 EAD 采用 Websocket 进行即时类消息服务的推送。

### JSON / JSONP

JSON（JavaScript Object Notation）是一种由道格拉斯·克罗克福特构想设计、轻量级的数据交换语言，以文字为基础，且易于让人阅读。尽管JSON是Javascript的一个子集，但JSON是独立于语言的文本格式，并且采用了类似于C语言家族的一些习惯。EAD 采用 JSON 进行服务端和客户端的主要数据交换。

### Stream

EAD 以流的方式对 GridFS 中的静态文件资源进行的访问，并对外以流的方式输出在线、附件或流媒体形式静态文件。