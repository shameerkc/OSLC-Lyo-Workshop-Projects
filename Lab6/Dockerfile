FROM maven
LABEL maintainer="shameer.kc@gmail.com"

# RUN apt-get --yes install git

# RUN git clone https://github.com/shameerkc/OSLC-Lyo-Workshop-Projects /opt/solr
# RUN cd /opt/solr/ninacrm; mvn install

RUN mkdir ~/lab6
COPY * ~/lab6

# EXPOSE 8181

CMD ["/bin/bash", "-c", "cd ~/lab6; mvn jetty:run"]
