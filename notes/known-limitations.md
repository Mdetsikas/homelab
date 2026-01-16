# Known Limitations & Planned Improvements

>This document tracks intentional limitations and future improvements for the homelab.
Not all features are implemented at once by design; this lab is built incrementally
to support learning and experimentation.

---

## Current Limitations

### Disk Metrics Visibility
- Some disk and root filesystem metrics are not fully visible in Grafana.
- This is due to node-exporter running in a container without full host filesystem mounts.
- Disk metrics will be expanded once host mounts are reviewed and intentionally exposed.

### Alerting
- Alerting is not currently configured.
- The focus at this stage is on understanding metrics and dashboards before introducing alerts.
- Alerting rules may be added after identifying meaningful signal vs noise.

### Authentication & Access Control
- Grafana is currently accessible within the home network.
- Advanced authentication (SSO, OAuth, or reverse proxy auth) is not yet configured.
- Access hardening will be evaluated once the dashboard layout stabilizes.

### Dashboard Organization
- Dashboards are currently using imported community templates.
- Panels and layouts will be refined as familiarity with metrics improves.
- Custom dashboards may be created later for lab-specific needs.

---

## Planned Improvements

- Refine disk and filesystem visibility
- Organize dashboards into folders by purpose
- Add basic alerting for system health
- Document Grafana configuration and dashboard choices
