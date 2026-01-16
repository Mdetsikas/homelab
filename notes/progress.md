# 🧭 Homelab Progress Log

> This log tracks major milestones, architectural decisions, and learning points.
> **Latest Update:** January 2026

---

## ✅ Phase 3: Container Observability & Visualization
**Focus:** Gaining visibility into Docker container performance.

- **Container Metrics:** Imported Docker/cAdvisor dashboards into Grafana.
- **Granularity:** Verified container-level visibility for CPU, memory, and network usage.
- **Organization:** Organized metrics under a dedicated "Containers" dashboard folder.
- **Validation:** Confirmed container discovery matches running services and documented expected N/A values for host-level metrics.

## ✅ Phase 2: Host Monitoring Stack
**Focus:** Establishing the "Three Pillars" of observability (Prometheus, Grafana, Node Exporter).

- **Visualizing Data:** Imported "Node Exporter Full" dashboard into Grafana.
- **Data Flow:** Validated end-to-end flow: `Exporters -> Prometheus -> Grafana`.
- **Health Checks:** Verified live CPU, memory, network, and load metrics for the Ubuntu VM.
- **Datasource Config:** Successfully connected Grafana to the Prometheus datasource.
- **Service Status:** Confirmed `node-exporter` and `cAdvisor` targets are UP in Prometheus.

## ✅ Phase 1: Core Infrastructure Setup
**Focus:** Provisioning the virtualization and container runtime environment.

- **VM Deployment:** Provisioned Ubuntu VM on Proxmox; verified network reachability.
- **Docker Strategy:** Chose VM-based Docker (nested) to keep the Proxmox hypervisor clean and isolated.
- **Health Check:** Verified basic container health using `docker ps`.

## 🚀 Project Initiation
- **Scope:** Defined homelab goals (Docker-first, observability-focused, moving to Kubernetes later).
- **Documentation:** Created initial GitHub repository structure and documentation standards.
- **Roadmap:** Prioritized Observability before complex orchestration.
