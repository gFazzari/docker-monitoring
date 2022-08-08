# Monitor Docker Containers

This solution offers the possibility to monitor your containers throught Prometheus metrics.
- Cadvisor and NodeExporter retrieve metrics from Docker Runtime and the host machine.
- Prometheus continues to fetch metrics and save them in a database.
- Grafana is connected to Prometheus and can query the databse and build usufull graphics based on tha data.
- AlertManager is a component of Prometheus that can send notification when certainly events are triggered.
- In this configuration AlertManager send the alerts to Calert, that is responsible to turn them over Google Chat Space.

Work based on: https://github.com/stefanprodan/dockprom