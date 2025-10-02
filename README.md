# Enclave Landscape Setup

## Docker

The docker-compose file spins up the following services:

- Grafana + Loki + Alloy (for logging and monitoring)
- Prometheus (for metrics collection)
- Meta DB (Postgres) (enduser and other meta data)
- Redis DB (for queue)

All monitoring services should come preconfigured and include Grafana dashboards
