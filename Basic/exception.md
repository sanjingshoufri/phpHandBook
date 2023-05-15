# Error
## 概述
- error type
	- System 
	- User
- 错误控制
	- php.ini(php-fpm) -> display_errors，如果这项没有打开，php脚本将没有任何输出	
- 错误提示
- stack trace
	- 提示信息列表的排序，从函数单位上来看底层在前，上层在后
	- 从真正代码行的级别来看，是按照代码执行的顺序的倒序来排序	

# Exception	
## 概述
- 异常机制
	- try
		- 在try代码块里的throw，不会直接抛出异常，而是由catch接收
		- 非try块里，就直接抛出异常了
	- 当出现异常时，异常之后的代码便不再执行了，php会尝试匹配catch块的代码