# Visually Enhanced Multi-Server Monitoring Dashboard

## Overview
This dashboard provides a comprehensive and visually appealing view of multiple servers using Node Exporter metrics collected by Prometheus.

## Features
- Real-time CPU and Memory usage trends
- Server metrics overview table with gradient gauges
- Disk usage distribution pie chart
- Network I/O bar graph
- Auto-refresh every 30 seconds

## Requirements
- Grafana 7.5+
- Prometheus datasource
- Node Exporter running on monitored servers

## Installation
1. Import the `dashboard.json` file into your Grafana instance.
2. Select your Prometheus data source when prompted.
3. Adjust the dashboard as needed for your environment.

## Metrics Used
- `node_cpu_seconds_total`
- `node_memory_MemTotal_bytes`
- `node_memory_MemAvailable_bytes`
- `node_filesystem_avail_bytes`
- `node_filesystem_size_bytes`
- `node_network_receive_bytes_total`
- `node_network_transmit_bytes_total`

## Customization
- Modify thresholds in panel settings to match your alerting needs.
- Add or remove panels by editing the dashboard JSON.
- Adjust the refresh rate in dashboard settings if needed.

## Support
For issues or feature requests, please file an issue on the GitHub repository.

## License
This dashboard is licensed under the MIT License.
