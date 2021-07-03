Spring 框架是 Java 应用最广的框架，它的成功来源于理念，而不是技术本身，它的理念包括 IoC (Inversion of Control，控制反转) 和 AOP(Aspect Oriented Programming，面向切面编程)。

Spring 的优势
低侵入 / 低耦合 （降低组件之间的耦合度，实现软件各层之间的解耦）
声明式事务管理（基于切面和惯例）
方便集成其他框架（如MyBatis、Hibernate）
降低 Java 开发难度
Spring 框架中包括了 J2EE 三层的每一层的解决方案（一站式）

Spring 能帮我们做什么
1.Spring 能帮我们根据配置文件创建及组装对象之间的依赖关系。
2.Spring 面向切面编程能帮助我们无耦合的实现日志记录，性能统计，安全控制。
3.Spring 能非常简单的帮我们管理数据库事务。
4.Spring 还提供了与第三方数据访问框架（如Hibernate、JPA）无缝集成，而且自己也提供了一套JDBC访问模板来方便数据库访问。
5.Spring 还提供与第三方Web（如Struts1/2、JSF）框架无缝集成，而且自己也提供了一套Spring MVC框架，来方便web层搭建。
6.Spring 能方便的与Java EE（如Java Mail、任务调度）整合，与更多技术整合（比如缓存框架）。



SpringMVC概念:
    他是一个轻量级的开源框架,应用于表现层,基于MVC的设计模式.
SpringMVC的特点:
    1.他是单例的可以设置成多例.
    2.他的线程是安全的 
    3.他是基于方法级别的拦截
    4.接受请求参数的方式是参数绑定
    5.携带参数到页面是通过request域对象.
SpringMVC流程
    1.用户向服务器发送一个请求,被SpringMVC的前端控制器DispatchServlet 捕获.
    2.DispatcherServlet接收到请求后调用HandlerMapping处理器映射器.
    3.处理器映射器找到具体的处理器(xml配置或者注解,RequesrtMapper),生成处理器对象及处理器拦截器一并返回给DispatcherServlet
    4.DispatcherServlet调用HandlerAdapter处理器适配器
    5.HandlerAdapter经过适配器调用具体的处理器(Controller)
    6.Controller执行完成后返回ModelAndView
    7.HandlerAdapter将Controller执行结果ModelAndView返回给DispatcherServlet
    8.DispatcherServlet将ModelAndView传给ViewReslover视图解析器
    9.ViewReslover解析后返回具体的View
    10.DispatcherServlet根据View进行渲染视图
    11.DispatcherServlet将渲染完的视图界面最后响应给用户.



Mybatis是一个对象关系映射（Object Relational Mapping，简称ORM）框架，是为了解决面向对象与关系数据库存在的互不匹配的现象。也就是说Mybatis的关注点在于对象与数据库之间的映射，Mybatis会把从数据库中得到的松散数据进行封装，使开发者直接拿到一个对象。Mybatis其实是对jdbc的操作数据库的过程进行了封装，使开发者只需要关注 SQL 本身，而不需要花费精力去处理例如注册驱动、创建connection、创建statement、手动设置参数、结果集检索等jdbc繁杂的过程代码。
Mybatis需要手写Sql语句，对jdbc的封装程度不如hibernate，但因此也灵活得多。
