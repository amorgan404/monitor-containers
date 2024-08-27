# Monitoring Setup with Prometheus, Grafana, and Node Exporter

This repository provides a simple setup for monitoring a Linux server using Prometheus, Grafana, and Node Exporter. The setup uses Docker Compose to orchestrate the services.

## Prerequisites

- Docker installed on your machine
- Docker Compose installed on your machine

## Services

- **Prometheus**: Collects and stores metrics.
- **Grafana**: Visualizes the metrics collected by Prometheus.
- **Node Exporter**: Exposes metrics about the host machine.

## Directory Structure

The repository has the following structure:

```
├── alertmanager.yml
├── docker-compose.yml
├── grafana
│   ├── dashboards
│   │   └── 1860_rev37.json
│   └── provisioning
│   ├── alerting
│   ├── dashboards
│   │   └── dashboards.yml
│   ├── datasources
│   │   └── datasource.yml
│   └── plugins
├── prometheus
│   ├── prometheus.yml
│   └── rules.yml
```


## Getting Started

1. **Clone the repository**

   ```bash
   git clone https://github.com/amorgan404/monitor-containers.git
   cd monitor-containers
   ```

2. **Start the services**
Use Docker Compose to start all the services:

   ```bash
   docker-compose up -d
   ```

3. **Access Grafana**
Open your browser and go to http://localhost:3000. The default login credentials are:
	- **Username**: admin
   - **Password**: admin
  
You will be prompted to change the password upon first login.

1. **Prometheus as a Data Source in Grafana**
Prometheus as a Data Sources and Grafana Dashboard have been added automatically.

## License

This project is licensed under the [LICENSE](https://github.com/amorgan404/monitor-containers/?tab=MIT-1-ov-file#) License.
