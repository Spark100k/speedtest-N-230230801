# speedtest-N-230230801
本项目是speedtest-N的修复版

speedtest-N地址https://github.com/ZenEcho/Speedtest-N

使用speedtest-N发现无法显示IP归属地和测速记录，所以修复上传了项目

部署：

下载本仓库并解压到网站目录。

1、访问 {域名}/index.html 进行测速

2、打开 {域名}/results.html 查看测速记录

3、results.html页面提示接口报错，是因为没有权限。请给予目录755权限（宝塔所有者权限是www非root）

Tips：backend/config.php 中可定义一些自定义配置：
MAX_LOG_COUNT = 100：最大可保存多少条测速记录
IP_SERVICE = 'ip.sb'：使用的 IP 运营商解析服务(ip.sb 或 ipinfo.io)
SAME_IP_MULTI_LOGS = false：是否允许同一IP记录多条测速结果
