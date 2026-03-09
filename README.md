# Monitoring System with Prometheus & Grafana

## 📌 Project Overview

This project demonstrates how to monitor a Spring Boot application using **Prometheus** and **Grafana**.

The system collects application metrics and visualizes them through a monitoring dashboard.

---

## 🧰 Tech Stack

* Spring Boot
* Prometheus
* Grafana
* Docker
* Micrometer

---

## 🏗 Architecture

Spring Boot Application
⬇
Prometheus (collect metrics)
⬇
Grafana (visualize metrics)

---

## 📊 Dashboard

Example monitoring dashboard:

![Grafana Dashboard](docs/grafana-dashboard.png)

The dashboard includes:

* HTTP Requests Per Second
* CPU Usage
* Application Uptime

---

## ⚙️ Setup & Run

### 1. Clone repository

```bash
git clone https://github.com/tathieungu/monitoring-project.git
cd monitoring-project
```

### 2. Start services

```bash
docker compose up -d
```

### 3. Access services

Prometheus

```
http://localhost:9090
```

Grafana

```
http://localhost:3000
```

Default login:

```
username: admin
password: admin123
```

---

## 📁 Project Structure

```
monitoring-project
|
├── 01-starter-files_db-scripts
├── 02-backend_spring-boot-rest-api
├── 03-frontend_angular-ecommerce
├── monitoring
│   ├── prometheus
│   │   └── prometheus.yml
│   │
│   └── grafana
│       ├── dashboards
|       |     └── system-app-dashboard.json
│       └──panel
|              |── App_uptime.png
|              |── CPU_usage.png
|              └── HTTP_Request_per_second.png
│
│
├── docker-compose.yml
└── README.md
```

---

## 📈 Metrics Collected

* HTTP request rate
* JVM memory usage
* CPU usage
* Application uptime

---

## 🚀 Future Improvements

* Add Alertmanager
* Add Loki for log monitoring
* Add Kubernetes monitoring

---

## 👨‍💻 Author

TaThieuNgu
