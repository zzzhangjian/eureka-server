# eureka-server
eureka-server 单机和集群

#单机启动
mvn clean install
java -jar eureka-server-0.0.1-SNAPSHOT.jar

#集群启动 
java -jar eureka-server-0.0.1-SNAPSHOT.jar --spring.profiles.active=7900
java -jar eureka-server-0.0.1-SNAPSHOT.jar --spring.profiles.active=7901
java -jar eureka-server-0.0.1-SNAPSHOT.jar --spring.profiles.active=7902


#配置security
# 1：关闭CSRF
# 2：配置密码
spring
  security:
    user:
      name: root
      password: root
