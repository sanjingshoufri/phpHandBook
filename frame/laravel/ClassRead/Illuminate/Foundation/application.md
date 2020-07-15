# Illuminate\Foundation\Application
## Class and Interface
extends和implement
- Illuminate\Container\Container
- Illuminate\Contracts\Foundation\Application

## property_list
- deferredServices                     延期服务和它们的提供者
- loadDeferredProvider                 

## method_list
- __construct()
	- setBasePath()
	- registerBaseBindings() 
- make()                               继承容器的make
- register()                           应用中注册一个服务提供

- isDeferredService()                  判断是否是延迟服务
- resolveProvider()                    实例化这个provider
- registerDeferredProvider()           注册一个延迟提供和服务

- dropStaleInstances()                 删除陈旧的实例和别名
- bindPathsInContainer()                       