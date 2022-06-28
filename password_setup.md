cd /usr/share/elk/docker-elk
docker exec docker-elk_elasticsearch_1 bin/elasticsearch-reset-password --batch --user elastic
docker exec docker-elk_elasticsearch_1 bin/elasticsearch-reset-password --batch --user kibana_system
Save exported password in .env file

docker restart docker-elk_kibana_1