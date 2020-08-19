1、连接VPS，执行以下命令

bash -c "$(curl -fsSL https://raw.githubusercontent.com/atrandys/trojan/master/trojan_mult.sh)"
2、选择1安装trojan

atrandys trojan一键脚本centos7+/ubuntu16.04+/debian9+

3、输入域名，不要带http或https，只输入域名即可，例如domain.com或 a.domain.com

4、设置trojan密码

atrandys trojan一键脚本centos7+/ubuntu16.04+/debian9+

5、下载配置好的win客户端或复制配置文件保存到本地

6、使用基本的win客户端，则直接运行start.bat即可开启代理，其他情况请使用5获取的配置文件自行启动trojan

常见问题
1、提示域名解析地址与本VPS IP地址不一致

如果你确认域名已经解析到VPS且没有开启CDN代理，可能的原因是你本地hosts文件中被系统默认添加了一条关于域名的解析（例如主机名填了当前使用的域名），使用cat /etc/hosts命令，若发现127.0.0.1 your_domian.com的记录，删掉即可；此问题也可以在脚本执行过程中选择强制安装解决。

更新记录
2020-08-18：

更新伪装站为电影题材模板
atrandys trojan一键脚本centos7+/ubuntu16.04+/debian9+
修改为手动设置trojan密码
acme.sh更换为nginx模式
修复自动更新证书功能
优化了部分存在问题的代码fork A大的trojan 一键脚本
系统要求及脚本介绍 1、系统>=centos7，用centos8最好，内核可直接开启bbr不需升级。
2、域名解析到VPS并生效。
3、脚本自动续签https证书
4、自动配置伪装网站，位于/usr/share/nginx/html/目录下，可自行替换其中内容
一、使用一键脚本安装 curl -O https://raw.githubusercontent.com/atrandys/trojan/master/trojan_centos7.sh && chmod +x trojan_centos7.sh && ./trojan_centos7.sh 另外建议安装bbr，以下脚本安装，不赘述了
cd /usr/src && wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh


1、连接VPS，执行以下命令

bash -c "$(curl -fsSL https://raw.githubusercontent.com/atrandys/trojan/master/trojan_mult.sh)"
2、选择1安装trojan

atrandys trojan一键脚本centos7+/ubuntu16.04+/debian9+

3、输入域名，不要带http或https，只输入域名即可，例如domain.com或 a.domain.com

4、设置trojan密码

atrandys trojan一键脚本centos7+/ubuntu16.04+/debian9+

5、下载配置好的win客户端或复制配置文件保存到本地

6、使用基本的win客户端，则直接运行start.bat即可开启代理，其他情况请使用5获取的配置文件自行启动trojan

常见问题
1、提示域名解析地址与本VPS IP地址不一致

如果你确认域名已经解析到VPS且没有开启CDN代理，可能的原因是你本地hosts文件中被系统默认添加了一条关于域名的解析（例如主机名填了当前使用的域名），使用cat /etc/hosts命令，若发现127.0.0.1 your_domian.com的记录，删掉即可；此问题也可以在脚本执行过程中选择强制安装解决。

更新记录
2020-08-18：

更新伪装站为电影题材模板
atrandys trojan一键脚本centos7+/ubuntu16.04+/debian9+
修改为手动设置trojan密码
acme.sh更换为nginx模式
修复自动更新证书功能
优化了部分存在问题的代码
