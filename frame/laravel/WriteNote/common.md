# IoC
## 概述
Ioc，Inversion of Control.

# Container
容器是管理类依赖的工具，通过依赖注入的方式来使用依赖类.

# Service Provider(服务提供者)
## 概述
服务提供者是Laravel
## property_list


## method_list
- register()
绑定操作:服务提供者被框架加载的时候，会检测它的属性和注册绑定.

- boot()
这个方法在所有的serviceProvider注册完后才执行的.

## 延迟提供者
为了实现延迟加载服务提供，implement \Illuminate\Contracts\Support\DeferrableProvider并且定义一个provides()，provides()应该返回服务容器绑定绑定注册.