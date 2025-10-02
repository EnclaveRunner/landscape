# Enclave Landscape Setup

## Docker Services

The docker-compose file spins up a complete monitoring and database stack with the following services:

### Services Overview

> [!WARNING]  
> These services are only for local testing, if run productively change default passwords!

| Service        | Port  | URL                    | Username            | Password           | Description                                                 |
| -------------- | ----- | ---------------------- | ------------------- | ------------------ | ----------------------------------------------------------- |
| **Grafana**    | 3000  | http://localhost:3000  | `admin`             | `admin`            | Dashboards & Visualization                                  |
| **Prometheus** | 9090  | http://localhost:9090  | -                   | -                  | Metrics Collection                                          |
| **Loki**       | 3100  | http://localhost:3100  | -                   | -                  | Log Aggregation                                             |
| **Alloy**      | 12345 | http://localhost:12345 | -                   | -                  | Log Collection Agent                                        |
| **cAdvisor**   | 8080  | http://localhost:8080  | -                   | -                  | Container Metrics                                           |
| **pgAdmin**    | 5050  | http://localhost:5050  | `admin@example.com` | `admin`            | PostgreSQL Web Interface (use pg password to add DB server) |
| **PostgreSQL** | 5432  | `localhost:5432`       | `enclave_user`      | `enclave_password` | Meta Database                                               |
| **Redis**      | 6379  | `localhost:6379`       | -                   | -                  | Queue                                                       |
