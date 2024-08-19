# Apache

## 基础介绍


### httpd
```yaml
httpd:

```


### 配置文件
```yaml
httpd.conf:
    Define: 定义变量
        ServerRoot: apache根目录
    DocumentRoot: 页面根目录
    ErrorLog: 错误日志位置
    Include: 导入其他配置文件
    KeepAlive: 连接保持
    Listen: 监听端口
    LoadModule: 加载动态库模块
    LogLevel: 日志级别
    MaxKeepAliveRequests: 长连接中可以传输的最大请求数量
    ServerAdmin:
    ServerName:
    <Directory>: 目录配置
        AllowOverride: 重写Apache配置
        Options: 启用服务器特性
        Require: 主机访问限制
    <IfModule>: 模块条件判断
    <VirtualHost>: 虚拟主机
        CustomLog:
        DocumentRoot:
        ErrorLog:
        ServerAdmin:
        ServerAlias:
        ServerName:
```

## 核心内容


### 虚拟主机

同时配置多个站点
