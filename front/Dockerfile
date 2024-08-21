#Setting java 8
FROM amazoncorretto:8u352-alpine
LABEL author=jlpinomoreno@gmail.com
RUN mkdir /home/admon_cfdi
RUN mkdir /home/admon_cfdi/resources
WORKDIR /home/admon_cfdi
COPY ./admon-cfdi-view.jar /home/admon_cfdi/app.jar
ENTRYPOINT ["java","-jar","/home/admon_cfdi/app.jar","--spring.config.location=/home/admon_cfdi/resources/application.properties"]
