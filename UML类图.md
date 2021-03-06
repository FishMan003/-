# 类的属性 #
在UML类图中，类使用包含类名、属性(field) 和方法(method) 且带有分割线的矩形来表示，比如下图表示一个Employee类，它包含name,age和email这3个属性，以及modifyInfo()方法。

![类的属性](http://images2015.cnblogs.com/blog/617148/201606/617148-20160612221055090-339746853.jpg)

· 	+ ：表示public

· 	- ：表示private

· 	#：表示protected

实际上，属性的完整表示方式是这样的：

可见性  名称 ：类型 [ = 缺省值]

# 类的方法的表示方式 #
可见性  名称(参数列表) [ ： 返回类型]

![类的方法](http://images2015.cnblogs.com/blog/617148/201606/617148-20160612222105058-2140837213.jpg)


# UML中的关系 #

## 依赖 Dependency ##

	带箭头的虚线表示，箭头从使用类指向被依赖的类。
	代码中一般指由局部变量、函数参数、返回值建立的对于其他对象的调用关系。
	一个类调用被依赖类中的某些方法而得以完成这个类的一些职责。

![依赖](http://www.uml.org.cn/oobject/images/3c13e1c1.jpg)

虚线箭头
 
##关联 Association##
	
	对象之间一种引用关系，比如客户类与订单类之间的关系。
	这种关系通常使用类的属性表达。
	关联又分为一般关联、聚合关联与组合关联。
	后两种在后面分析。
	在类图使用带箭头的实线表示，箭头从使用类指向被关联的类。可以是单向和双向。
	
	实线箭头	
1. 单向关联
		
	![单向关联](http://images2015.cnblogs.com/blog/617148/201606/617148-20160612224805636-1840590061.jpg)
2. 双向关联
	
	![双向关联](http://images2015.cnblogs.com/blog/617148/201606/617148-20160612225006840-13774319.jpg)

	双方各自持有对方类型的成员变量
3. 自关联
	
	![聚合关系](http://images2015.cnblogs.com/blog/617148/201606/617148-20160612225421496-664373564.jpg)

	自己包含自己
##聚合 Aggregation##
	
	
![聚合关系](http://images2015.cnblogs.com/blog/617148/201606/617148-20160612225421496-664373564.jpg)


	空心菱形和箭头表示
	整体包含部分,部分可脱离整体单独存在
	比如上图中汽车包含了发动机，而发动机脱离了汽车也能单独存在。
## 合成 Composition

![合成关系](http://images2015.cnblogs.com/blog/617148/201606/617148-20160612232819824-829657559.jpg)

显然，嘴是头的一部分且不能脱离了头而单独存在。在UML类图中，组合关系用一个带实心菱形和箭头的直线表示。
##泛化 (继承) Generalization

![泛化(继承)](http://images2015.cnblogs.com/blog/617148/201606/617148-20160612233246199-1404301867.jpg)


##实现 Realization

![](http://images2015.cnblogs.com/blog/617148/201606/617148-20160612233430777-736506858.jpg)

虚线三角



# 类图符号 #

## 类 ##

长方形，由3部分组成，第一部分类名、第二部分属性、第三部分方法。

   ![类](http://www.uml.org.cn/oobject/images/image001.gif)

## 包 ##

![包](http://www.uml.org.cn/oobject/images/image002.gif)

## 接口 ##

通常使用带有名称的小圆圈表示

![接口](http://www.uml.org.cn/oobject/images/image003.gif)