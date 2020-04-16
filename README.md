# store-server

这是[闪鲤电商小程序私有化部署](https://minapp.dev)的服务端

> 当前服务端版本: v1.1.0

## 准备事项

* 确保你已获得license
* 确保你已将域名解析至你的服务器IP
* 确保你的服务器开放了80和443端口

## 如何部署

1. 下载服务端

    ```
    $ git clone https://github.com/minappdev/store-server.git
    $ cd store-server
    ```

3. 编辑config.env文件

    ```
    # 根据配置文件内的注释完成配置: 小程序, 微信商户, 腾讯云短信, 腾讯云cos, 高德地图, mysql, redis等
    ```

4. 启动服务端

    ```
    $ sudo ./store-server ./config.env

    # 成功启动后会打印: 管理后台地址及小程序后台需要配置的相关服务器域名
    # 你可以使用nohup或其他工具让store-server在后台运行
    ```

## 服务端对外网络请求的说明

* 高德, 地图API
* 微信, 小程序API
* 易联云, 打印小票. (如果你添加小票打印机的话)
