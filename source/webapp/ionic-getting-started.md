title: 模板应用入门介绍
---

## 目录结构

```
├── bower.json // Bower 配置文件
├── config.xml // 应用配置文件
├── gulpfile.js
├── hooks
├── ionic.config.json // Ionic 配置文件
├── node_modules // NPM 模块安装目录
├── package.json // NPM 包配置文件
├── platforms //应用平台目录
├── plugins // Cordova、Ionic 插件目录
├── res
├── resources
├── scss
└── www
    ├── css
    ├── img
    ├── index.html
    ├── js
    │   ├── app.js
    │   ├── controllers.js
    │   └── services.js
    ├── lib
    │   └── ionic
    ├── manifest.json
    ├── service-worker.js
    └── templates
```

## 根目录

### config.xml

Ionic 应用配置文件，配置 App 名称、各平台资源路径、应用内容、作者信息等。

### platforms

平台资源文件目录，用于应用打包的资源或源代码，执行添加平台命令后会自动下载。

### plugins

Cordova、Ionic 插件目录，执行添加插件命令后会自动下载。

### res

多分辨率资源目录，可以根据自己的项目需要替换图片。

### resources

App 启动资源目录，可以根据自己的项目需要替换图片。

## WWW 目录

WWW 目录为 Ionic 项目内容目录，```index.html``` 为默认内容入口，所有的 UI 界面、业务逻辑、数据服务都在该目录下进行。

### www/index.html
Ionic 默认内容入口，如果需要调整请在项目根目录下的 ```config.xml``` 文件中修改。

### www/js/app.js
Inoic 模板应用默认应用配置和注册文件，在该文件中进行应用模块和路由的初始化。

### www/js/controllers
Ionic 模板应用默认控制器文件，在该文件中注册定义应用视图控制模块。

### www/services.js
Ionic 模板应用默认数据服务文件，在该文件中注册定义应用服务模块。

### www/templates
Ionic 模板应用默认模板文件目录，在该目录存储用户交互界面模板文件。

## 创建新界面

### 添加视图控制器

### 添加视图模板

### 配置视图路由

## 创建新数据服务

### 添加数据服务

### 绑定数据

#### 模块依赖

#### $scope

#### 模板指令

- ng-model
- ng-repeat
- ng-if
- ng-show
- ng-hide