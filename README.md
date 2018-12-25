# TOOLS
	工具集

## 向日葵ubuntu配置方法
	传送门：https://ywnz.com/linuxrj/2965.html：
	[下载地址]（https://sunlogin.oray.com/zh_CN/download/）
	装向日葵客户端 for Linux教程

		1.下载

		打开上面下载地址，选择“Linux”系统，点击“免费下载”。

		2.解压

		（下列步骤以Centos系统为例，命令以管理员身份运行）

		下载完成后，进入对应下载目录，输入命令将压缩包解压本地：

		tar xzvf SunloginClient9.6.1.tar.gz

		3.绿色版

		输入 cd sunloginclient_packet/ 进入解压后目录；

		输入 ./run.sh 即可运行绿色版，默认只有快访远控功能，暂不支持开机自启动；

		快访远控功能：主控端只需通过被控端生成的快访码与验证码即可发起远控。
		 输入 ./run.sh stop 则是停止绿色版服务启动；

		输入 ./run.sh help 则是查看脚本命令帮助。
		 4.正式版（支持开机自启动）

		输入 cd scripts/ 进入正式版安装目录；

		输入 ./install.sh 安装向日葵Linux被控端；输入./uninstall.sh则是卸载。
		输入 ./start.sh 启动向日葵服务（输入./stop.sh 停止向日葵服务）；

		启动成功显示配置链接：http://主机IP:30080 ，浏览器打开该链接进行配置。

		注：30080端口为向日葵被控端Web配置端口，安全考虑建议禁止对外开放此端口。
