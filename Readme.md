# ELK.

### Задание 1. Elasticsearch

___Установите и запустите Elasticsearch, после чего поменяйте параметр cluster_name на случайный. Приведите скриншот команды 'curl -X GET 'localhost:9200/_cluster/health?pretty', сделанной на сервере с установленным Elasticsearch. Где будет виден нестандартный cluster_name.___

Docker

cluster_name=docker-cluster

![docker elasticsearch](./img/2025-01-13_16-28-09.png)

```bash
docker exec -it elk-elasticsearch-1 /bin/bash
nano config/elasticsearch.yml
```

```
cluster.name: "custom_cluster"
```

![custom cluster_name](./img/2025-01-13_16-31-18.png)


### Задание 2. Kibana

___Установите и запустите Kibana. Приведите скриншот интерфейса Kibana на странице http://<ip вашего сервера>:5601/app/dev_tools#/console, где будет выполнен запрос GET /_cluster/health?pretty.___

![kibana console](./img/2025-01-13_17-01-00.png)


### Задание 3. Logstash.

![logstash](./img/2025-01-13_20-25-52.png)


### Задание 4. Filebeat.

![filebeat](./img/2025-01-13_21-44-30.png)