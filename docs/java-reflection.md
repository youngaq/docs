# Java反射

什么是反射:

Java反射机制是在运行状态中，能够知道任何一个类的所有属性和方法；对于任何一个对象，都能够调用它的任意方法和属性；这种动态获取信息以及动态调用对象方法的功能称为java语言的反射机制。

允许程序在运行时通过反射取得任何一个已知名称的class的内部信息，包括其modifiers（诸如public、static等）、superclass（例如Object）、实现之interfaces（例如Cloneable），也包括fields和methods的所有信息，并可于运行时改变fields内容或唤起methods。反射可以在运行时加载、探知、使用编译期间完全未知的classes。

反射能做什么:

反射（reflection）允许静态语言在运行时（runtime）检查、修改程序的结构与行为。

可以利用反射技术实现反射实现动态代理，热加载。
