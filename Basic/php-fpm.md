# PHP-FPM
## 概述
- PHP与PHP-FPM协同工作，之间有两种通信方式unix socket和tcp socket

## 优化
- 背景
	- 优化PHP-FPM可以提高NGINX的性能
- 配置FPM(php-fpm.conf)
	- emergency_restart_threshold 10
		- 重启设置
	- process_control_timeout
		- 告诉子进程等待接收父进程的时间
- 配置www.conf
	- pm
		- Dynamic
			- 定义最小和最大值
		- Static
			- 无论发生什么，都有固定数量的PHP数量进程
		- ondemand
			- 通过指令创建和销毁