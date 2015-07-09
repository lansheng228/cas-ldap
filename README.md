在cas-overlay基础上, 根据文档配置的支持oauth 2.0协议的服务端。
cas文档：http://jasig.github.io/cas/4.0.x/index.html
cas构建基础：https://github.com/lansheng228/cas-overlay
构建命令：mvn clean package
将生成的war包，放到/var/lib/tomcat7/webapps/下， 重启tomcat。

在ldap上新建目录，并建立测试数据。
根据实际情况配置cas.properties中的ldap管理员用户名和密码,以及其他项。

访问https://localhost:8443/cas，进入登录界面，输入测试的用户名和密码，登录成功。
