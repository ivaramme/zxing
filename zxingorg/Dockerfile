FROM tomcat:8
 
RUN rm -rf /usr/local/tomcat/webapps/ROOT
COPY src/main/webapp/.ebextensions/server.xml /usr/local/tomcat/conf/server.xml
COPY target/zxingorg-3.3.3.war /usr/local/tomcat/webapps/ROOT.war
