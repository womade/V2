## V2H-DEV
[![](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

### V2H
- [x] 支持 vmess 和 vless 两种协议
- [x] 支持自定义 WebSocket 路径
- [x] 伪装首页
- [x] HTML5 测速
- [x] 使用 v2 最新版构建

请求`/`，返回3D元素周期表

请求`/speedtest/`，html5-speedtest 测速页面

请求`/test/`，文件下载速度测试

请求`/ray`（可配置）v2ray WebSocket 路径


### 环境变量说明

|  名称 | 值  | 说明  |
| ------------ | ------------ | ------------ |
|  PROTOCOL |  vmess<br>vless（可选） |  协议：nginx+vmess+ws+tls 或是 nginx+vless+ws+tls |
|  UUID |  [uuid在线生成器](https://www.uuidgenerator.net "uuid 在线生成器") | 用户主 ID  |
|  WS_PATH | 默认为`/yuanzheng` |  路径，请勿使用`/speedtest`，`/`，`/test` 等已经被占用的请求路径 |

### 进阶
[uptimerobot](https://uptimerobot.com/) 定时访问防止休眠