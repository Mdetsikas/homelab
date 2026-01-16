# Personal Homelab

## Overview
This repository documents my personal homelab environment.
The goal of this lab is to build hands-on experience with
virtualization, containerization, and observability tooling
in a controlled, internal-only environment.

This lab is intentionally small and iterative, focusing on
learning fundamentals rather than building a production-grade system.

---

## Hardware
- Repurposed gaming PC hardware
- Single-node setup

---

## Virtualization
- Hypervisor: Proxmox
- Purpose: Host VMs and containers for experimentation

---

## Current Focus: Dashboard & Monitoring

I am currently building an internal dashboard and monitoring stack to
better understand observability concepts.

### Components (In Progress)
- Docker
- Prometheus (metrics collection)
- Grafana (visualization)

This stack is being built incrementally to better understand how
metrics flow from services to dashboards.

---

## Design Philosophy
- Internal-only services
- Docker-first to learn container fundamentals
- Everything is documented and replaceable
- Break things intentionally, then fix them

---

## Current Status
- Proxmox host is operational
- Docker is being used for service deployment
- Monitoring stack is actively being built

---

## Lessons Learned
_(This section will grow as the lab evolves.)_

---

## Future Plans
- Improve dashboard organization
- Add alerting
- Explore logging solutions
- Re-evaluate architecture as skills grow
