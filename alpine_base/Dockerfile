FROM alpine:python

ENV JANA=/configs
ENV APP_CONFIG=/app/local/conf/apps_conf/jpbs-service
ENV CATALINA_CONFIG=/usr/local/tomcat

RUN mkdir -p /app/local/conf/apps_conf/jpbs-service/certs && \
    mkdir -p /usr/local/tomcat/conf && \
    ln -s ${JANA}/log4j.xml ${APP_CONFIG}/log4j.xml && \
    ln -s ${JANA}/ProcessorMappings.xml ${APP_CONFIG}/ProcessorMappings.xml && \
    ln -s ${JANA}/dynamic.properties ${APP_CONFIG}/dynamic.properties && \
    ln -s ${JANA}/secure.properties ${APP_CONFIG}/secure.properties && \
    ln -s ${JANA}/static.properties ${APP_CONFIG}/static.properties && \
    ln -s ${JANA}/tomcatConnector.xml ${APP_CONFIG}/tomcatConnector.xml && \
    ln -s ${JANA}/ach_deb_email_report_en_US.properties ${APP_CONFIG}/ach_deb_email_report_en_US.properties && \
    ln -s ${JANA}/jpbs-ssl.p12 ${APP_CONFIG}/certs/jpbs-ssl.p12 && \
    ln -s ${JANA}/vault-client.p12 ${APP_CONFIG}/certs/vault-client.p12 && \
    ln -s ${JANA}/catalina.policy ${CATALINA_CONFIG}/conf/catalina.policy && \
    ln -s ${JANA}/catalina.properties ${CATALINA_CONFIG}/conf/catalina.properties && \
    ln -s ${JANA}/logging.properties ${CATALINA_CONFIG}/conf/logging.properties && \
    ln -s ${JANA}/context.xml ${CATALINA_CONFIG}/conf/context.xml && \
    ln -s ${JANA}/server.xml ${CATALINA_CONFIG}/conf/server.xml && \
    ln -s ${JANA}/tomcat-users.xml ${CATALINA_CONFIG}/conf/tomcat-users.xml && \
    ln -s ${JANA}/tomcatConnector.xml ${CATALINA_CONFIG}/conf/tomcatConnector.xml && \
    ln -s ${JANA}/web.xml ${CATALINA_CONFIG}/conf/web.xml
