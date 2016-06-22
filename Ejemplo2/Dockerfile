FROM websphere-liberty:kernel
MAINTAINER Emilio J Alarcon <ejalarcon@gmail.com>
ENV LICENSE accept
COPY server.xml /config/
COPY server.env /config/
RUN installUtility install --acceptLicense defaultServer
RUN mkdir -p /de/qpri/online/multipais/web/logs
RUN chmod 777 /de/qpri/online/multipais/web/logs
RUN mkdir -p /de/qpri/online/multipais/web/cfg
RUN chmod 777 /de/qpri/online/multipais/web/cfg
RUN mkdir -p /de/qpri/online/multipais/web/cfg/entorno
RUN chmod 777 /de/qpri/online/multipais/web/cfg/entorno
