# 概述
- composer是PHP的一个依赖管理工具，它允许你声明项目所依赖的代码库，它会在你的项目中安装他们
- composer.json
	- Key
		- autoload
			- PSR4定义【命名空间】到【路径】的映射
			- autoload的值，起到映射关系解析和加载类文件的作用
				- 类文件只有类实例化的时候才加载