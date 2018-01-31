<https://e-hentai.org> 本子下载脚本，自用

## 使用方式

执行：`node ./download <url> [path]`

参数:

- url：本子详情页面的URL，不要漏了协议名

- path：保存的文件夹路径，路径不存在会自动创建，默认为当前工作目录

## 已知问题

在下载图片时，如果与下载服务器成功建立连接，但服务器一直不返回主体数据，这时程序会一直等待

request模块貌似并没有提供read timeout的选项，现在临时的解决方案就是重启程序后继续下载

## TODO

- [x] 使用作品名自动创建文件夹
- [x] 账号登录
- [x] 下载原图
- [ ] 范围下载
- [x] 保存下载进度记录
- [x] 使用进度记录继续下载
- [x] 通过SOCKS(5)代理下载
- [x] 对exhentai的支持
- [ ] 解决图片有时下载不完整的问题