# geeker-hiwifi
对于极路由的深度研究
目前手头上root的机器是极1S，极路由内置了Nigix服务提供的后台，配合Lua脚本提供openapi与客户端通信，DHCP和DNS使用的是Dnsmasq
- 下载 工程模式 插件 获取 ssh 访问ssh登陆权限
  - `ssh -p 1022 admin@ip` 密码是路由器后台密码
- 使用curl下载https的文件 机器上面没找到内置的证书 需要下载一个
 - 下载 cacert.pem.zip 并解压. 百度云盘 http://pan.baidu.com/s/1qYMRB0C
 - `curl --cacert /path/to/cacert.pem  -L -O https://want.to.com/file`
