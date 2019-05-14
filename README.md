# Monitoring Applications and Services: an ELK approach

The current repository contains a dockerized implementation of the following services:
* Elasticsearch
* Kibana
* Metricbeat
* Logstash
* Elastalert
* NGINX (optional)

## How to start the docker containers

1) Replace all variables inside <...> with their correct values depending on your host configurations/slack_hook/etc.
2) Place all directories listed in this repository into the /opt folder (or replace /opt in docker-instalation/docker-compose-METRICS.yml )
3) Run the following command (assuming you have docker and docker-compose installed in your machine):

```
docker-compose -f docker-compose-METRICS.yml up -d elasticsearch kibana metricbeat logstash elastalert ngnix

```

For more information on the overall architecture and this specific implementation, refer to https://medium.com/@manuelmourato25/elk-stack-alerting-how-to-monitor-your-business-and-infrastructure-data-part-one-a4a1c3427745