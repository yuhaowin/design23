适配器模式:
定义: 将一个类的接口转换成客户期的另一个接口;
使得原本不兼容的类可以一起工作;
类型,结构型;

适用的场景:对于已经存在的类,其方法和需求不匹配时

注意:适配器模板不是在在软件设计的阶段应该考虑的设计模式,而是随着软件的发展,在软件的维护过程中,由于不同的产品,不同的厂家造成的
功能类似,而接口不同情况下的解决方案;


适配器模式的优点:

能够提高类的透明性和复用性,使得现有的类得到复用,而不需要做出改变,
目标类和被适配的解耦,提高程序的扩展性;


符合开闭原则,具体的实现都在适配器中,被客户端知道的只有适配器,扩展的时候只需要扩展适配器类即可;

缺点:

适配器编写的过程中需要全面的考虑,可能会增加系统的复杂性,
增加代码的可阅读性;

如果使用过多的适配器,会使得代码逻辑变得很混乱;



适配器模式的扩展:

对象适配器:
  符合组合复用原则,使用委托机制
  
  
类适配器:
  通过类的继承实现
  
  
适配器相关的设计模式
  适配器和门面(外观)模式  
  
  
  jdk中的使用的适配器:
  
  xmlAdapter
    
  