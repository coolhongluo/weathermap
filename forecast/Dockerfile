FROM 100.125.5.235:20202/caoyongsheng/dockerhub-java:8-jre-alpine


WORKDIR /home/apps/
ADD target/forecast-1.0.0.jar .
ADD target/lib ./lib
ADD start.sh .

ENTRYPOINT ["sh", "/home/apps/start.sh"]
