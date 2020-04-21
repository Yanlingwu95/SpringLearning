# Day1：Spring基本概念

## Quick insight：

1. Spring是一个开源轻量级框架
2. Spring核心：
   1. AOP：面向切面编程， 扩展功能不是修改源代码实现
   2. IOC：控制反转：
      - 比如有一个类，在类里有一个方法，（不是静态的）调用类的方法，创建类的对象，使用对象调用方法，创建类对象的过程，需要new一个对象；
      - 把对象的创建，不是通过new的方式实现，而是交给spring配置创建类对象；
3. Spring是一站式框架：
   1. Spring在java的三层结构中，每一层都提供不同的解决技术：
      - web层： spring MVC
      - service层：spring的IOC
      - dao层：spring的jdbc template（java database connectivity)

---

### Spring的IOC操作：

1. 把对象的创建交给spring管理

2. ioc操作两部分：

3. 1. ioc的配置文件的方式
   2. ioc的注解方式

### IOC底层原理：

1. ioc底层原理使用的技术

2. 1. xml配置文件
   2. dom4j解析xml
   3. 工厂设计模式
   4. 反射

![1](C:\Users\yanli\Desktop\1.PNG)