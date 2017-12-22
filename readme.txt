包括
1. 整合Mybatis
http://localhost:8080/student/listAll
http://localhost:8080/student/create?name=heu30u90e&age=32
http://localhost:8080/student/find?name=heu30u90e
http://localhost:8080/student/list

PageHelper分页插件
http://localhost:8080/student/page?pageNum=1&pageSize=1

之前调试不通
@Configuration
public class MyBatisConfiguration

http://localhost:8080/student/part?pageNum=1&pageSize=1

2. 常用的配置
# 项目contextPath，一般在正式发布版本中，我们不配置
server.context-path=/sb   (http://localhost:9090/sb/)
# tomcat最大线程数，默认为200
server.tomcat.max-threads=800
# tomcat的URI编码
server.tomcat.uri-encoding=UTF-8
# 错误页，指定发生错误时，跳转的URL。请查看BasicErrorController源码便知
server.error.path=/error
# 服务端口
server.port=9090
# session最大超时时间(分钟)，默认为30
server.session-timeout=60
# 该服务绑定IP地址，启动服务器时如本机不是该IP地址则抛出异常启动失败，只有特殊需求的情况下才配置
# server.address=192.168.16.11



3. 项目打包
e:
cd E:\hx_workspace\springboot3
mvn clean package
在项目target目录下找到war包