# Namespace Configuration
- **Namespace Creation**:
  - Enabled: true
- **Namespace Name**: sre-msockperf-exporter

# Environment Domain Configuration
- **Environment Domain**: msockperf.domainname.com

# Labels Configuration
- **Labels Enabled**: true
- **Owner Label**: "sre"

# Ingress Configuration
- **Ingress Enabled**: false

# ServiceMonitor Configuration
- **ServiceMonitor Enabled**: true

# Portworx Configuration
- **Portworx Enabled**: false

# Rancher Configuration
- **Rancher Enabled**: false
- **Rancher Project ID**: [empty]

# msockperf Configuration
- **Service Name**: msockperf-service
- **App Name**: msockperf-app
- **Docker Image**: ghcr.io/aetrius/msockperf-client/msockperf-client:main
- **Replica Count**: 1
- **Revision History Limit**: 0
- **Web Port**: 8082
- **Namespace**: default
- **Remote Host**: sockperf-server-service.sre-msockperf-exporter
- **Remote Port**: 3600
- **Service Port**: 8000
- **Image Pull Policy**: Always

# sockperfServer Configuration
- **Service Name**: sockperf-server-service
- **App Name**: sockperf-app
- **Docker Image**: ghcr.io/aetrius/msockperf-server/msockperf-server:main
- **Replica Count**: 1
- **Revision History Limit**: 1
- **Sockperf Port**: 3600
- **Web Port**: 3600
