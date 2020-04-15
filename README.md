# store-server

这是[闪鲤电商小程序私有化部署](https://minapp.dev)的服务端

> 当前服务端版本: v1.1.0

## 准备事项

* 确保你已获得license
* 确保你已将域名解析至你的服务器IP
* 确保你的服务器开放了80和443端口

> 依赖: 小程序, 微信商户, 腾讯云短信, 腾讯云cos, 高德地图, mysql, redis. 配置文件内有详细注释

## 如何部署

1. 下载适用于Linux amd64的服务端

```
$ curl https://raw.githubusercontent.com/minappdev/store-server/master/store-server -o store-server
$ chmod +x store-server
```

2. 下载配置文件
```
$ curl https://raw.githubusercontent.com/minappdev/store-server/master/config.env -o config.env
```

3. 编辑config.env文件

```
# 根据配置文件内的注释完成配置
```

4. 启动服务端

```
$ ./store-server ./config.env
# 成功启动后会打印: 管理后台地址及小程序后台需要配置的相关服务器域名
# 你可以使用nohup或其他工具让store-server在后台运行
```
