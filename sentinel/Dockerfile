FROM adoptopenjdk/openjdk8

MAINTAINER scjava@qq.com

RUN mkdir -p /sc/sentinel

WORKDIR /sc/sentinel

EXPOSE 8080

ADD ./sentinel-dashboard-1.8.7.jar ./app.jar

ENTRYPOINT ["java", "-Dserver.port=8080", "-Dcsp.sentinel.dashboard.server=localhost:8080", "-Dproject.name=sentinel-dashboard", "-Dsentinel.dashboard.auth.password=sentinel#sc2024QWE!"]

CMD ["-jar","app.jar"]
