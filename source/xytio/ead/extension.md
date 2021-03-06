title: 扩展驱动
---
![扩展驱动](.\images\extend-driver.png)

EAD 专注于解决 80% 简单重复且可配置的应用开发问题，在运行生命周期的各个关键节点都允许开发者自定义开发扩展驱动，以应对各种可能出现的复杂需求和应用场景。

如上图所示，从服务端到客户端的数据传输环节一共有 6 个节点允许自行开发扩展驱动，在 EAD 引擎和 Rainbow 中分别以依赖注入和闭包回调的方式动态加载和执行扩展驱动。

### EAD 引擎

EAD 引擎端允许根据需求和场景利用 Java 语言扩展开发系统变量驱动、查询驱动、视图驱动、视图动作驱动，通过驱动管理组件注册后可以在开发者应用中心配置选择。

### Rainbow

Rainbow 核心任务是负责视图用户交互界面的渲染和动作交互界面的渲染，允许开发者利用 JavaScript 自定义视图扩展驱动和动作扩展驱动，将扩展 JS 文件放置到指定目录即可在开发者配置中心以文件命名空间的形式配置动作执行自定义扩展驱动。