> 官网 https://railway.app 每月500小时试用期，官方明确说明了禁止磁力下载、大流量传输，封号误怪！

- 协议：vless + ws, tls在平台最外层网关已经做掉了，当然你也可以改为vmess、trojan等协议
- ws路径： /api
- 用户uuid： 详见config.yaml


代码中没有加保活策略，该平台为docker容器，理论上进程没那么容易死掉，如果web（xray）挂掉了，请自行get请求一下`https://你的域名/start`。   
  
<br>
貌似最近注册的github账号是没法在平台认证通过的，绑卡又挺麻烦，建议用老github账号。导入该项目后，平台不会自动生成域名，需要点一下面板中项目的方框->Settings->Environment->Generate Domain。大概过2~5分钟，再访问该域名，不出意外就会出现hello world ,然后再请求一下/start，即可开启xray
<br>
<br>

- /start  启动xray
- /info   查看系统信息
- /status 查看系统进程表

 
