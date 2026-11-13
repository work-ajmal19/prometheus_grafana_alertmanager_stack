About the stack
Prometheus is a metrics database. It scrapes (pulls) numeric metrics like CPU,
memory and request counts from targets at regular intervals and stores them as time
series.

Grafana is the dashboard tool. It connects to Prometheus as a data source and draws
graphs and dashboards.

Alertmanager receives alerts fired by Prometheus rules (for example, CPU above
80%) and routes them to email, Slack, PagerDuty and so on, with grouping and
silencing.

Node Exporter (added here) exposes host machine metrics so Prometheus has
something to scrape.

Why used: This is the standard open source monitoring stack for servers, containers
and Kubernetes clusters. Prometheus collects, Grafana visualizes, Alertmanager
notifies