FROM tomcat:8-jre7
ENV CATALINA_BASE /usr/local/tomcat
COPY tomcat-users.xml $CATALINA_BASE/conf/tomcat-users.xml
COPY context.xml $CATALINA_BASE/conf/context.xml
COPY arq-spring.tar $CATALINA_BASE/lib/
RUN cd $CATALINA_BASE/lib/ && tar -xvf arq-spring.tar && rm arq-spring.tar
COPY probe.war $CATALINA_BASE/webapps/probe.war
RUN mkdir -p /de/qqqq/online/multipais/web/logs
RUN chmod 777 /de/qqqq/online/multipais/web/logs
RUN mkdir -p /de/qqqq/online/multipais/web/cfg
RUN chmod 777 /de/qqqq/online/multipais/web/cfg
RUN mkdir -p /de/qqqq/online/multipais/web/cfg/entorno
RUN chmod 777 /de/qqqq/online/multipais/web/cfg/entorno
