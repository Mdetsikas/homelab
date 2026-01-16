## Architecture (High-Level)

```mermaid
graph TD
    A[Proxmox Host] --> B[Ubuntu VM]
    B --> C[Docker]
    C --> D[Prometheus]
    D --> E[Grafana]
