# HTTP
## method
- $\_post
	- http的post方法
	- 自动全局变量

- $GLOBALS['HTTP_RAW_POST_DATA']
		- 总是生产$HTTP_RAW_POST_DATA
			- 包含原生的OST数据
		- 当遇到未定义的MIME类型数据
			- 比如$HTTP_RAW_POST_DATA  for  enctype="multipart/form-data"
				- 这个格式的数据是不可用的