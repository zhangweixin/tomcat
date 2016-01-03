# tomcat source调试project
## 1.简单介绍
这是一个调试tomcat源代码的基于maven的project;
在idea或者eclipse下面直接导入project即可使用;
project使用的tomcat源码版本7.0.47
## 2.project 运行设置
Tomcat的启动入口为org.apache.catalina.startup.Bootstrap，这个类运行时候会为tomcat容器的
初始化做一系列必要参数收集以及设定。
### 下面是Bootstrap这个类启动时必要设置的VM参数:
-Dcatalina.home=catalina-home
-Dcatalina.base=catalina-home
-Djava.endorsed.dirs=catalina-home/endorsed
-Djava.io.tmpdir=catalina-home/temp
-Djava.util.logging.manager=org.apache.juli.ClassLoaderLogManager
-Djava.util.logging.config.file=catalina-home/conf/logging.properties


