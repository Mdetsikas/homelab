# Docker Compose Strategy

## Overview
This homelab uses **Docker Compose** to manage services running inside an **Ubuntu VM** on a Proxmox host.

The goal is to keep deployments:
- reproducible (easy to rebuild)
- organized (clear service boundaries)
- safe to iterate on (easy to roll back)

---

## Why Docker Compose
Docker Compose is being used instead of individual `docker run` commands because it:
- keeps the full stack in one place (services, networks, volumes)
- makes upgrades and restarts consistent
- documents intent in a readable format
- simplifies troubleshooting and recovery

---

## File & Directory Layout (Planned)

````
docker/
├── compose.yml
├── env/
│   └── example.env
├── prometheus/
│   ├── prometheus.yml
│   └── rules/ (future)
└── grafana/
    └── provisioning/ (future)
````

Notes:
- Secrets and environment-specific values should not be committed directly.
- Use `.env` locally and commit an `example.env` template instead.

---

## Services (Initial Stack)
- **Prometheus** (metrics collection)
- **Grafana** (visualization)

Future additions may include:
- Alerting (Alertmanager or equivalent)
- Logging (Loki, etc.)

---

## Networking Approach
- Services communicate on a dedicated Docker network.
- External exposure is minimized (internal-only where possible).
- Published ports are documented in the README when used.

---

## Persistence / Volumes
- Prometheus and Grafana will use volumes so data survives container restarts.
- Volume locations and backup approach will be documented as the stack stabilizes.

---

## Change Management
- Small changes, committed often
- Document why changes were made (not just what changed)
- Keep the stack easy to rebuild from scratch
