# WebWX

网页微信协议说明

## 登录

登录相关的信息由服务器 `login.wx.qq.com` 来处理的。

登录信息相关的 API 调用可以通过如下地址来访问：

[http://petstore.swagger.io/?url=https://raw.githubusercontent.com/TommyLau/WebWX/master/login.wx.qq.com.yaml](http://petstore.swagger.io/?url=https://raw.githubusercontent.com/TommyLau/WebWX/master/login.wx.qq.com.yaml)

包含的方法：

| 方法 | 操作 | 概要 |
| ---- | ---- | ---- |
| /jslogin | GET | 获取微信登录所需要的 UUID |
| /qrcode/{uuid} | GET | 生成登录 QR Code |
| /cgi-bin/mmwebwx-bin/login | GET | 扫描 QR Code |

## 初始化

初始化相关的信息是由 `wx.qq.com` 来处理的。

> 其实这个地址有好几个，比如 `wx2.qq.com`、`wx8.qq.com` 等等，主要根据最后登录成功后返回的 `redirect_uri` 来决定。

相关 API 调用参考如下地址：

[http://petstore.swagger.io/?url=https://raw.githubusercontent.com/TommyLau/WebWX/master/wx.qq.com.yaml](http://petstore.swagger.io/?url=https://raw.githubusercontent.com/TommyLau/WebWX/master/wx.qq.com.yaml)

包含的方法：

| 方法 | 操作 | 概要 |
| ---- | ---- | ---- |
| /cgi-bin/mmwebwx-bin/webwxinit | POST | 初始化网页微信 |

## 消息处理

To be updated
