#This Dockerfile builds Apache JMeter Slaves/Server Executable
FROM vishnumurty/jmbase
MAINTAINER vishnumurty
LABEL Description="This image is used to start the Apache JMeter Slaves/Server Executable"

# Ports to be exposed from the container for JMeter Slaves/Server
EXPOSE 1099 50000

# Application to run on starting the container
ENTRYPOINT $JMETER_HOME/bin/jmeter-server \
                        -Dserver.rmi.localport=50000 \
                        -Dserver_port=1099
