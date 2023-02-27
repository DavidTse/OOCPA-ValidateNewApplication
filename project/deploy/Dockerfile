FROM registry.access.redhat.com/ubi8/openjdk-11:latest
COPY image-files /
EXPOSE 8090
WORKDIR /
CMD ["sh","-c", "java -Xms128m -Xmx512m -XX:+UseParallelOldGC -XX:MinHeapFreeRatio=10 -XX:MaxHeapFreeRatio=20 -Dorg.kie.server.mode=PRODUCTION -jar /OOCPA-ValidateNewApplication-1.0.0-SNAPSHOT.jar"]