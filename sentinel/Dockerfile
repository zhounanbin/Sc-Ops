FROM adoptopenjdk/openjdk8

MAINTAINER scjava@qq.com

RUN mkdir -p /sc/sentinel

WORKDIR /sc/sentinel

EXPOSE 8080

ADD ./sentinel-dashboard-1.8.7.jar ./app.jar

ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "app.jar"]

CMD ["-Dserver.port=8858", "-Dcsp.sentinel.dashboard.server=localhost:8858", "-Dproject.name=sentinel-dashboard", "-Dsentinel.dashboard.auth.password=sentinel#sc2024QWE!"]
