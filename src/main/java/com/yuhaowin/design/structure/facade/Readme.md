外观模式(门面模式)

提供一个统一接口,用来访问子系统中的一群接口

外观模式定义了一个高层接口,让子系统更容易访使用.

类型:结构性;

角色:外观角色,外观角色了解子系统的所有的方法,也要自己的方法,客户端通过调用外观角色的方法来调用子系统的功能.

子系统:子系统可以是一个或者是多个,子系统形成一个集合为外观类提供服务


外观模式的适用场景:

1 子系统越来越复杂,增加外观模式提供简单的接口调用

2 在构建多层系统结构,利用外观对象作为每层的入口,简化层间的调用.

通过不同的外观类可以达到对不同的软件版本有不同的调用逻辑;

外观模式的优点:

简化了调用过程,无需深入了解子系统,防止带来风险.

减少系统依赖,松散耦合,客户端不和子系统直接交流,只和外观对象直接交流,使得子系统内部各个模块更加容易扩展和维护.

更好的划分访问层次.把需要暴露给外部的功能集中到外观类上,既方便客户端的调用,又很好的隐藏了细节.

符合迪米特法则,(最少知道原则) 外观模式是迪米特法则的最典型的例子

外观模式的缺点:

增加子系统.扩展子系统的行为时容易引发风险.

不符合开闭原则.

相关设计模式: 外观模板与中介者模式;

外观模式关注的是外界和子系统之间的交互,
中介者模式关注的是子系统内部之间的交互

外观模式和单例模式
通常将外观模式中的外观类设计成单例的


外观模式和抽象工厂模式:

外观类可以通过抽象工厂获取子系统的实例,子系统可以将内部对外界屏蔽


注意:客户端一定只能和外观类进行交流,不能和子系统进行交流.


外观模式在jdk 和 开源框架中的使用. JdbcUtils 和  tomcat 大量使用 facade模式 