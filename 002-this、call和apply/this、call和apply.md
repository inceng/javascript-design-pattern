
具体示例demo参考 index.html

# this

## this指向

1.作为对象的方法调用

当作为对象的方法调用时，this指向该对象。

2.作为普通函数调用
当作为普通函数调用时，this总是指向全局对象。即window

3.构造器调用
当使用构造器new创建实例后，该实例中的this指向用new生成的对象。

4.Function.prototype.call 或 Function.prototype.apply调用

此时，可以动态的更改this ，指向新的上下文根（新的对象  context）


# call和apply

## apply
func.apply(context,[arg1,arg2...]) 

## call
func.apply(context,arg1,arg2...) 

call是包装在apply上的语法糖（实际上的实现还是通过apply实现的）。

call和apply主要作用是改变this的指向，即改变上下文根。修正不正确的this指向。
