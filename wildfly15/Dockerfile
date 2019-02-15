FROM jboss/wildfly:latest
ADD customization /opt/jboss/wildfly/customization/
RUN /opt/jboss/wildfly/customization/execute.sh
RUN /opt/jboss/wildfly/bin/add-user.sh admin admin --silent
CMD ["/opt/jboss/wildfly/bin/standalone.sh", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0"]
EXPOSE 8080:8080
#ADD your-awesome-app.war /opt/jboss/wildfly/standalone/deployments/