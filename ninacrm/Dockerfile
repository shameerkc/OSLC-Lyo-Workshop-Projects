FROM maven
LABEL maintainer="shameer.kc@gmail.com"

# RUN apt-get --yes install git

# RUN git clone https://github.com/shameerkc/OSLC-Lyo-Workshop-Projects /opt/solr
# RUN cd /opt/solr/ninacrm; mvn install

RUN mkdir ~/ninacrm
COPY * ~/ninacrm

# EXPOSE 8181

CMD ["/bin/bash", "-c", "cd ~/ninacrm; mvn clean install jetty:run"]
