FROM tomcat:8.5
ADD https://s3-us-west-2.amazonaws.com/studentapi-cit/student.war /usr/local/tomcat/webapps
ADD https://s3-us-west-2.amazonaws.com/studentapi-cit/mysql-connector.jar lib/mysql-connector.jar
COPY context.xml conf/context.xml 
WORKDIR ./bin

EXPOSE 8080

CMD ["./catalina.sh", "run"]
