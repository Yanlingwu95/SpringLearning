## 基于aspectj的注解AOP

1. 使用注解方式实现AOP操作

   第一步： 创建对象：

   ````
   <!-- 创建对象-->
   <bean id= "book" class = "File.Path.To.Class.Book"></bean>
   <bean id= "myBook" class = "File.Path.To.Class.MyBook"></bean>
   ````

   第二步： 在spring核心配置文件中，开启AOP操作

   ```
   <!-- 开启AOP操作 -->
   <aop:aspectjautoproxy></aop:aspectjautoproxy>
   ```

   第三步 使用注解完成增强配置

   ```
   @Aspect
   public class MyBook {
       //在方法上面使用注解完成增强配置
       @Before(value="execution(* File.Path.To.Class.Book.*(..))")
       public void before1() {
           System.out.println("before.....");
       }
   }
   ```
