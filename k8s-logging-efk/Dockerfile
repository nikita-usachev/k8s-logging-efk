# Logging with ElasticSearch

# Website docker.elastic.co
# Docker pull elasticsearch

FROM docker.elastic.co/elasticsearch/elasticsearch:version

# Elasticsearch configuration

COPY elasticsearch.yml /usr/share/elasticsearch/config/elasticsearch.yml

# User account

USER elasticsearch

# Elasticsearch data directory

VOLUME /usr/share/elasticsearch/data
