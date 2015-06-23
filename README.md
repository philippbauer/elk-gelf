## ELK GELF

Docker image of ELK stack (Elasticsearch + Logstash + Kibana) with GELF input support.
This repo was forked of fayndee/elk-logback!

### Get started

1. Pull the docker image: `docker pull philippbauer/elk-gelf`
2. Run the docker container: `docker run -d -p 9200:9200 -p 12201:12201 -p 5601:5601 philippbauer/elk-gelf`

### Embedded configuration

Service ports are configured as below and are exposed by default.

port | protocol | service       | description                  
---- | -------- | ------------- | ---------------------------
9200 | TCP      | Elasticsearch | Elasticsearch service port.  
12201| TCP      | Logstash      | Logstash GELF input port.     
5601 | TCP      | Kibana        | Kibana UI port.              

