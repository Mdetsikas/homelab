# Homelab Progress Log

## Milestone 1
- Created initial GitHub documentation
- Defined scope and goals for the homelab
- Decided to focus on Docker and observability before Kubernetes

## Next Steps
- Stand up Prometheus using Docker
- Connect Grafana to Prometheus
- Document service connectivity

---

## Milestone 2
- Confirmed Docker is running inside an Ubuntu VM on the Proxmox host
- Chose VM-based Docker to keep the Proxmox host clean and isolate lab services
- Next focus: stand up Prometheus + Grafana and document the data flow

---

## Milestone 3
- Ubuntu VM is running on Proxmox and reachable from the home network
- Docker is installed and operational inside the VM
- Initial dashboard services are running and accessible via the VM IP
- Verified basic container health using `docker ps`

---

## Milestone 4
- Prometheus and Grafana containers are running without errors
- node-exporter and cAdvisor containers are active and healthy
- Prometheus targets page confirms all exporters are UP
- Verified Prometheus is successfully scraping metrics from all configured targets

---

## Milestone 5
- Added Prometheus as a datasource in Grafana
- Confirmed Grafana can query Prometheus successfully
- Validated end-to-end metrics flow from exporters to Prometheus and Grafana
- Prepared environment for dashboard visualization and analysis

---

## Milestone 6
- Imported Node Exporter Full dashboard into Grafana
- Verified live CPU, memory, network, and load metrics
- Confirmed real-time observability of the Ubuntu VM
- Identified optional disk metrics enhancements for future refinement

---


