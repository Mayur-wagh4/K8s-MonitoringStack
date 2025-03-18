# Observability-For-DevOps

## Overview
Observability-For-DevOps is a **comprehensive monitoring and observability solution** designed for **DevOps engineers** to gain deep insights into their infrastructure and applications. This stack integrates **Prometheus, Grafana, cAdvisor, and Node Exporter** for real-time data collection, visualization, and performance analysis.

Additionally, a **custom monitoring demo app** is included to showcase observability in action.

## Features
- **Real-time performance monitoring** of containers, servers, and applications.
- **Pre-configured dashboards** in Grafana for instant visibility.
- **Automated metrics collection** with Prometheus.
- **Container resource tracking** using cAdvisor.
- **Hardware and OS-level insights** via Node Exporter.
- **Persistent data storage** for Prometheus and Grafana.

## Tech Stack
- **Docker & Docker Compose** → Containerized deployment
- **Prometheus** → Time-series metrics collection
- **Grafana** → Advanced visualization & dashboards
- **cAdvisor** → Container-level resource monitoring
- **Node Exporter** → OS and hardware monitoring
- **Demo App** → Showcases the observability capabilities

## Installation

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Mayur-wagh4/K8s-MonitoringStack.git
cd K8s-MonitoringStack
```

### 2️⃣ Install Docker & Docker Compose
- [Docker Installation Guide](https://docs.docker.com/get-docker/)
- [Docker Compose Installation Guide](https://docs.docker.com/compose/install/)

### 3️⃣ Deploy the Monitoring Stack
```bash
docker compose up -d
```

## Usage
- **Grafana Dashboard** → [http://localhost:3000](http://localhost:3000)
  - Default credentials: `admin` / `admin`
- **Prometheus UI** → [http://localhost:9090](http://localhost:9090)
- **cAdvisor Metrics** → [http://localhost:8080](http://localhost:8080)
- **Node Exporter Metrics** → [http://localhost:9100/metrics]
- **Demo Monitoring App** → [http://localhost:8000]

## Services
- **Prometheus** → Stores and manages time-series metrics
- **Grafana** → Provides visualization and dashboards
- **cAdvisor** → Collects container performance metrics
- **Node Exporter** → Exposes system-level metrics
- **Demo App** → Simulates real-world observability use cases

## Persistent Data Storage
- `prometheus_data` → Stores Prometheus metrics persistently.
- `grafana_data` → Stores Grafana dashboards & configurations.

## Networking
- **monitoring-network** → Isolated network for secure service communication.

## Troubleshooting
🔹 **Check logs if a service fails to start:**
```bash
docker logs <container_name>
```
🔹 **Restart a service:**
```bash
docker restart <container_name>
```
🔹 **Check running containers:**
```bash
docker ps
```
🔹 **Verify Prometheus targets:**
```bash
curl http://localhost:9090/api/v1/targets
```

## Contributing
Contributions are welcome! Feel free to **submit a pull request** or **open an issue** to enhance this project.

## License
This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

