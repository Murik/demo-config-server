

docker run -it -p 8888:8888 -p 5015:5015 -v "C:\Work\imp\demo-config-server\src\main\resources\config":/config -e SPRING_PROFILES_ACTIVE=native -e JAVA_OPTS=-agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=*:5015 hyness/spring-cloud-config-server:2.2.6.RELEASE-jdk11 