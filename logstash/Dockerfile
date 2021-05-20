FROM docker.elastic.co/logstash/logstash:7.12.1

RUN rm -rf /usr/share/logstash/pipeline
COPY pipeline /usr/share/logstash/pipeline
COPY config/ /usr/share/logstash/config/
RUN logstash-plugin install logstash-output-elasticsearch
