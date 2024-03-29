# kual-wifi-transfer

依赖于 KUAL 和 Python3 的 Kindle 插件，用于 WiFi 传书到 Kindle。

基本原理是在 Kindle 上运行一个 HTTP Server，这样局域网内的电脑、手机等设备访问一个 `http://<kindle 的局域网 IP>:8000` 的地址，就可以打开一个可以上传电子书到 Kindle 的网页。

## 运行效果

Kindle 端插件运行效果：

<img width="320px" src="./screenshots/kindle-extension.png"/>

电脑端上传页面效果：

<img width="640px" src="./screenshots/page-to-upload.png"/>

手机端上传页面效果：

<img width="320px" src="./screenshots/page-to-upload-mobile.png"/>

## 安装方法

该插件依赖于 KUAL 和 Python3，请确保之前已经正确安装它们。它们的安装方法可以参考 <https://bookfere.com/post/311.html>。

本插件安装方法：

1. 下载本项目代码，可以用 git clone，也可以到 [releases](https://github.com/mzlogin/kual-wifi-transfer/releases) 下载；

2. 将 Kindle 用数据线连接电脑，把上面下载的代码里的 wifi-transfer 文件夹拷贝到 Kindle 的 /mnt/us/extensions 目录下。

## 使用方法

1. 在 Kindle 上打开 KUAL，就可以在插件列表里看到「WiFi Transfer」菜单项了，点击「Start Server」，Kindle 上将显示 `Starting server at <ip:port>`；

2. 在电脑或手机上访问第 1 步显示的 `<ip:port>`，选择电子书文件并上传。

## 适用机型

当前只在 Kindle PaperWhite 一代上运行过，其它机型未验证，理论上也适用。

- Kindle PaperWhite

## License

[MIT License](./LICENSE)
