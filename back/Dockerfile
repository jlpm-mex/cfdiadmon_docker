FROM amazoncorretto:17-alpine3.23

LABEL author="jlpinomoreno@gmail.com"

RUN mkdir -p /home/admon_cfdi/resources
WORKDIR /home/admon_cfdi

RUN wget -O /home/admon_cfdi/app.jar https://github.com/jlpm-mex/cfdiadmon/releases/download/0.0.2-SNAPSHOT/admon-cfdi-back-0.0.2-SNAPSHOT.jar

ENTRYPOINT ["java","-jar","/home/admon_cfdi/app.jar","--spring.config.location=/home/admon_cfdi/resources/application.properties"]
