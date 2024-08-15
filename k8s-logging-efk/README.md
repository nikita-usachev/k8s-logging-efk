# Logging with ElasticSearch

---

## What is EFK?

- ElasticSearch
- Fluentd
- Kibana

---

## Why choose EFK over ELK?

- EFK: ElasticSearch, Fluentd, Kibana

- ELK: ElasticSearch, Logstash, Kibana

1. Log aggregators and analysis tools. Logging stack:

- Logs exporter
- Log collector
- Logs storage
- Logs visualization

2. Event Routing:

- EFK: Routed on tags (much easier)
- ELK: if-else condition

3. Plugins:

- EFK: Plugins hosted elsewhere
- ELK: Centralized GitHub repository

4. Transport:

- EFK: Safer, has configurable in-memory
- ELK: In-memory queue of 20 events, needs Redis for persistence across restart.

5. Performance and high-volume logging:

- EFK: Written in Ruby, scales very well, fast
- ELK: Consumes more memory

6. Log Parsing:

- EFK: Standard built-in parsers (JSON, regex, csv, etc.)
- ELK: Plugins

7. Docker support:

- EFK: Docker has built in logging driver for Fluentd.
- ELK: Requires plugin (filebeat) to read application logs.

8. Which one to use for Kubernetes?

- Fluentd has built-in Docker logging driver and parser.
- Doesn't require extra agent.
- Less complex and less mistakes.
- Fluentd and Kubernetes are both CNCF project.

CNCF: Cloud Native Computing Foundation
