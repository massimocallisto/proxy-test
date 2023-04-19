FROM tomcat:8.5 AS tomcat_base

RUN mkdir /opt/tomcat/

WORKDIR /usr/local/tomcat/webapps
RUN curl -O -L https://github.com/AKSarav/SampleWebApp/raw/master/dist/SampleWebApp.war


FROM tomcat_base AS app1
RUN mv SampleWebApp.war app1.war

FROM tomcat_base AS app2
RUN mv SampleWebApp.war app2.war


#EXPOSE 8080


#CMD ["catalina.sh", "run"]
