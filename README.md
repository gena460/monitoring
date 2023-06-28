# monitoring


# monitoring

Розгорніть моніторинговий стек для вашого проєкту.

Компоненти:

OpenTelemetry

Prometheus

Fluentbit

Grafana Loki

Grafana

Оцінювання:

(junior): Стек розгорнуто та налаштовано у локальному  dev-середовищі для демо проєкту за допомогою docker-compose

https://github.com/den-vasyliev/kbot/blob/opentelemetry/otel/docker-compose.yaml 

(middle): Стек розгорнуто та налаштовано у dev-середовищі в Kubernetes для власного проекту. Fluentbit збирає та експортує логи проєкту та всіх нод кластеру.

(senior): Стек розгорнуто та налаштовано у dev-середовищі в Kubernetes для власного проєкту за допомогою Flux. Otel розгорнуто оператором. Fluentbit збирає та експортує логи проєкту та усіх нод кластеру. Проєкт інструментовано для експорту метрик.

(principal): Проект інструментовано з наскрізним TraceID


-------------------------------------------



# Monitoring Stack for Your Project

This repository contains the code and configuration for deploying a monitoring stack in your local dev environment using Docker Compose. The stack includes the following components:

- OpenTelemetry
- Prometheus
- Fluent Bit
- Grafana Loki
- Grafana

## Deployment Instructions

1. Install Docker and Docker Compose on your local machine.

2. Clone this repository:

   ```bash
   git clone https://github.com/gena460/kbot.git
Navigate to the directory with the Docker Compose file:

bash
Copy code
cd kbot/otel
Start the monitoring stack using Docker Compose:

bash
Copy code
docker-compose up -d
Once the stack is successfully launched, you can access various components:

OpenTelemetry: http://localhost:4317
Prometheus: http://localhost:9090
Grafana: http://localhost:3002 (login: admin, password: admin)

## Grafana Demo Dashboard

![Image](.data/dashboard.png)
