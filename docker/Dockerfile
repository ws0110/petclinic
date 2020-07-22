FROM tomcat:9.0.30-jdk8-openjdk

RUN ln -snf /usr/share/zoneinfo/Asia/Seoul /etc/localtime \
    && echo "Asia/Seoul" > /etc/timezone
    
COPY ./petclinic.war /usr/local/tomcat/webapps/ROOT.war

EXPOSE 8080

CMD ["catalina.sh","run"]

# Image Build
# docker build --tag ws0110/petclinic:0.1 .
