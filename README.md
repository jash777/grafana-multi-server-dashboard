# Visually Enhanced Multi-Server Monitoring Dashboard

![Grafana](https://img.shields.io/badge/Grafana-7.5%2B-orange)
![Prometheus](https://img.shields.io/badge/Prometheus-2.0%2B-red)
![License](https://img.shields.io/badge/License-MIT-blue)
![Version](https://img.shields.io/badge/Version-1.0.0-green)

A comprehensive and visually appealing Grafana dashboard for monitoring multiple servers using Node Exporter metrics collected by Prometheus.

![Dashboard Screenshot](dashboard1t.png)

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Metrics](#metrics)
- [Customization](#customization)
- [Contributing](#contributing)
- [Support](#support)
- [License](#license)

## Features

- Real-time CPU and Memory usage trends with smooth line graphs
- Server metrics overview table with gradient gauges for quick status checks
- Disk usage distribution visualized in an interactive pie chart
- Network I/O activity displayed in a dynamic bar graph
- Auto-refresh every 30 seconds for up-to-date information
- Responsive layout suitable for various screen sizes
- Dark theme optimized for NOC and data center environments

## Requirements

- Grafana 7.5+
- Prometheus 2.0+
- Node Exporter running on monitored servers

## Installation

1. Ensure you have Grafana and Prometheus set up in your environment.
2. Install Node Exporter on all servers you wish to monitor.
3. Clone this repository:
   ```
   git clone https://github.com/jash777/grafana-multi-server-dashboard.git
   ```
4. In Grafana, navigate to "Create" > "Import".
5. Either upload the `dashboard.json` file or copy and paste its contents into the "Import via panel json" field.
6. Select your Prometheus data source when prompted.
7. Click "Import" to finalize the dashboard setup.

## Usage

After installation, you can start using the dashboard immediately. Here's how to make the most of it:

1. **Server Overview**: The main table provides a quick glance at all your servers' vital stats.
2. **CPU and Memory Trends**: Use these graphs to identify patterns or anomalies over time.
3. **Disk Usage**: The pie chart helps visualize storage distribution across servers.
4. **Network Activity**: Monitor network I/O to detect unusual traffic patterns.

To add more servers, simply ensure they're running Node Exporter and are scraped by your Prometheus instance. The dashboard will automatically include them.

## Metrics

This dashboard utilizes the following Node Exporter metrics:

- `node_cpu_seconds_total`
- `node_memory_MemTotal_bytes`
- `node_memory_MemAvailable_bytes`
- `node_filesystem_avail_bytes`
- `node_filesystem_size_bytes`
- `node_network_receive_bytes_total`
- `node_network_transmit_bytes_total`

## Customization

You can customize this dashboard to better fit your needs:

- Adjust thresholds: Edit panel settings to change the color thresholds for different metrics.
- Modify refresh rate: Change the auto-refresh time in the dashboard settings.
- Add new panels: Incorporate additional metrics or visualizations as needed.
- Change time range: Use Grafana's time picker to view data over different periods.

## Contributing

We welcome contributions to improve this dashboard! Here's how you can contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them with a clear, descriptive message.
4. Push your changes and submit a pull request.

Please ensure your code adheres to the existing style and that all tests pass before submitting a pull request.

## Support

If you encounter any issues or have questions, please:

1. Check the [Issues](https://github.com/jash777/grafana-multi-server-dashboard/issues) page to see if it's already been addressed.
2. If not, open a new issue with a clear description and, if possible, steps to reproduce the problem.

For general questions, feel free to start a discussion in the [Discussions](https://github.com/jash777/grafana-multi-server-dashboard/discussions) section.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ by [Jashuva/alphasec]
