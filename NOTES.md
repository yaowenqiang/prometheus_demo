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

### WMI Exporter

+ Windows Management Instrumentation
+ Not avaiable on Official Prometheus website

https://github.com/prometheus-community/windows_exporter


## Metric types

+ Counter - A counter is a cumulative metric that represents a single monotonically increasing counter whoese value can only increase or be reset to zero on restart
+ Gauge - A gauge is a metric that represents a single numerical value that can arbitrarily go up and down
+ Histogram - A histogram samples observations (usually things like request durations or reponse size) and counts them in configurable buckets, it also provides a sum of all observed values
+ Summary - Similar to a histogram, a summary samples observations,(usually things like request durations and response sizes), While it also provides a total count of observations and a sum of all observed values, it calculates configurable quantilies over a sliding time window.

Gauge are typically used for measured values like temperatures or current memory usage, but also 'counts' that can go up and down, like the number of concurrent requests





curl "localhost:5006?[1-10]"
