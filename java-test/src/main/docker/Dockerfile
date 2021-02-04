#使用jdk8作为基础镜像
FROM openjdk:8-jdk-alpine
#指定作者
MAINTAINER Ron.lin
#暴露容器的端口
EXPOSE 5000
#将复制指定的gateway-java-sample-code-1.0.jar为容器中的mpgs.jar，相当于拷贝到容器中取了个别名
ADD gateway-java-sample-code-1.0.jar mpgs.jar
#
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/mpgs.jar"]