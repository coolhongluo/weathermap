FROM 100.125.5.235:20202/caoyongsheng/dockerhub-java:8-jre-alpine

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone

WORKDIR /home/apps/
ADD target/weather-beta-2.0.0.jar .
ADD target/lib ./lib
ADD start.sh .

ENTRYPOINT ["sh", "/home/apps/start.sh"]
