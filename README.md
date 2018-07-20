# huan-swagger
## 项目结构
 huan-swagger-core  swagger核心组件封装
 
 huan-swagger-ui    swagger UI页面，作为一个第三方服务来渲染接口，用来渲染远程服务器的接口说明  10.6.51.135:8102
 
 huan-swagger-test  swagger 微服务测试页面  10.6.51.135:8101
 
 访问形式：http://10.6.51.135:8102/webjars/swagger-ui/index.html#10.6.51.135:8101


## 使用说明
 1、 spring boot项目启动项添加：
 
    @EnableHuanSwagger
    
 2、 pom依赖
  
    <dependency>
        <groupId>com.huanshare</groupId>
        <artifactId>huan-swagger-core</artifactId>
        <version>1.0.0-SNAPSHOT</version>
    </dependency>

 3、页面访问：UI服务器地址/webjars/swagger-ui/index.html#API-服务器地址
 
 ## 特点
  
  原来看过别人的源码，直接将swagger 部署在API服务上，无法实现API，UI分离
  
  现在这种方式实现了API与UI的分离，但是需要为UI单独部署一套服务器，增加了其他成本
  
  如果微服务多的话，这也算是个不错的方案
  
    