# 入口文件
## 类相关(调用顺序)
- Illuminate\Foundation\Application
	- registerBaseBindings
	- registerBaseServiceProviders()
	- registerCoreContainerAliases()
	- make()
	- 

- Illuminate\Contracts\Http\Kernel(interface)
	- bootstrap()，
	- handle()，
	- terminate()，
	- getApplication()，

## 备注
1. 打印各个类的调用关系.