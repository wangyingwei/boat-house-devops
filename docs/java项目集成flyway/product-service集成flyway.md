Product-service服务集成flyway插件操作步骤

1、在pom.xml文件中，添加依赖

![](../images/flyway-int1.png)

其中jdbc链接驱动版本号（5.1.2），本次测试需要添加，本地mysql数据库版本号5.7.9，更高版本数据库，没有进行测试。

![](../images/flyway-int2.png)

2、在pom.xml文件中，添加新的插件

![](../images/flyway-int3.png)

3、修改数据库链接参数配置文件

![](../images/flyway-int4.png)

4、在resource/db目录下，新建数据库版本控制文件/migration/V1.0\_\_init.sql

![](../images/flyway-int5.png)

5、清空数据表，运行程序，进行测试

运行前

![](../images/flyway-int6.png)

运行后

![](../images/flyway-int7.png)

![](../images/flyway-int8.png)

![](../images/flyway-int9.png)

6、添加新的数据库版本文件，进行测试

![](../images/flyway-int10.png)

![](../images/flyway-int11.png)

![](../images/flyway-int12.png)
