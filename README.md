## 为什么要使用ngrok？

> 作为一个Web开发者，我们有时候会需要临时地将一个本地的Web网站部署到外网，以供他人体验评价或协助调试等等，通常我们会这么做：

1. 找到一台运行于外网的Web服务器
1. 服务器上有网站所需要的环境，否则自行搭建
1. 将网站部署到服务器上
1. 调试结束后，再将网站从服务器上删除

只不过是想向朋友展示一下网站而已，要不要这么麻烦，累感不爱╰（`□′）╯

-----

## 有了ngrok之后，世界是如此的美好

1. 首先[下载](windows_amd64.zip)`ngrok`
1. 运行命令`ngrok -config=ngrok.cfg -subdomain demo 8080`，`demo`是自定义子域名，不带`-subdomain demo`时会随机生成一串字符作为子域名，`8080`是你本地Web服务的端口
    ```
    ngrok                                                                                                                   (Ctrl+C to quit)
    
    Tunnel Status                 online
    Version                       1.7/1.7
    Forwarding                    http://demo.dev.baylittle.com:86 -> 127.0.0.1:8080
    Forwarding                    https://demo.dev.baylittle.com:86 -> 127.0.0.1:8080
    Web Interface                 127.0.0.1:4040
    # Conn                        0
    Avg Conn Time                 0.00ms
    ```
1. 你会得到一串网址`http://demo.dev.baylittle.com:86`，其中`:86`不要带入浏览器地址，直接通过`http://demo.dev.baylittle.com`这个网址就可以访问你本地的Web服务了

-----

## 获取ngrok

[windows 64位](windows_amd64.zip)

-----

##

> 服务器是自己的，大家如果用的开心，捐个一毛两毛的，我也感激不尽了（尴尬笑）

<img src="https://i.loli.net/2017/11/06/5a0025bb0029c.jpg" alt="微信" width="300" />
