# monitor phase

+ Data Colection
+ Data Storage
+ Data Visualization
+ Alerting
+ Analytics & Reporting

## Exporter

+ A Prometheus Exporter is a piece of software that an statistics from another non-Prometheus system
+ Can turen these statistics into Prometheus metrics, using a client library

### Node Exporter

+ Node Exporter is Prometheus official exporter for hardware and kernel-related metrics
+ It expose kernel-level and machine-level metrics on unix/linux system
+ It provides metrics like CPU, Memory, Disk space, Disk I/O and network bandwidth etc.

default node exporter port is 9100

metrics start with node_

rate(node_cpu_seconds_total{mode="system"}[1m])





