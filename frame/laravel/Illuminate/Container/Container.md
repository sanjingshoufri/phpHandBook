# Illuminate\Container\Container
## property
- with[]              重载参数栈
- buildStack          
- abstractAliases     抽象类的别名
- extenders           service拓展包
- instances           容器中的共享实例
- bindings[]          绑定
- contextual          上下文绑定映射

## method_list
- singleton()，容器内注册一个共享绑定(只实例化一次).

- make()/resolve()，容器中解析给定的抽象类.
    - build()，实例化一个具体类.
    - resolveDependencies()，从反射参数中解析所有的依赖.

- resolved()，判断给定的抽象类型是否已经解析.

- instance()         在容器中注册一个共享实例.

- getConcrete()，抽象类的具体类.
	- getContextualConcrete()，抽象类的上下文的具体绑定.
		- findInContextualBindings()，contextual属性中取值.

- getLastParameterOverride()，上一个重写参数.

- bind()    容器中注册一个绑定.
- build()   实例化具体类.

- getClosure()，    

- alias()，
	- 这个方法是什么时候调用的