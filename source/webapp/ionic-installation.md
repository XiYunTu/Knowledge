title: 开发环境安装
---


## 安装依赖

### Node.js & NPM

Ionic 以及 Cordova 安装依赖于 Node.js 和 NPM 包管理器，如果你没有安装请前往 [Node.js](http://nodejs.org)官方网站下载合适的版本（建议安装最新版本）进行安装。

> NPM 全局（-g）模块安装注意事项：
> - MacOS 请使用 sudo 命令；
> - Windows 请使用管理员身份运行命令行窗口。

### Cordova

```
npm install -g cordova
```

> Cordova 官方网址：https://cordova.apache.org/

## Ionic CLI

### 安装

```
npm install -g ionic
```

### 创建应用

切换文件目录到你要创建应用的父目录下，执行如下命令创建 Ionic 应用：
```
ionic start myApp tabs
```

> $ ionic start myapp [template]
> 
> - myapp - 应用名称（会在当前目录下创建同名目录）
> - template - 模板
>   - tabs (默认)
>   - sidemenu
>   - blank


### 启动 Web 服务

切换到应用目录下，执行如下命令启动 Web 服务：
```
cd myapp
ionic serve
```

### 添加目标平台

Android
```
ionic platform add android
```

iOS
```
ionic platform add ios
```

### 模拟器运行

### 应用打包