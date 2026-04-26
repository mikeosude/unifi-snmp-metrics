# unifi-snmp-metrics

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Status: Active](https://img.shields.io/badge/status-active-brightgreen.svg)]()

Unlock visibility into your UniFi infrastructure. This repository provides curated SNMP OID mappings to monitor the disk health and performance of your UniFi hardware, specifically tested for the **UniFi UNAS Pro 4** and **UDM-SE**.

## 🚀 Why this project?
Standard SNMP monitoring often misses the proprietary OIDs required to get granular health data from UniFi storage devices. This project bridges that gap, allowing you to feed actionable health metrics into your observability stack.

## 🛠️ Supported Hardware
* **UniFi UNAS Pro 4**
* **UniFi Dream Machine Special Edition (UDM-SE)**
* *Have another device? Pull requests are welcome!*

## 📈 Integration
Designed to work seamlessly with:
* **Prometheus SNMP Exporter**
* **Grafana** (for visualization)
* **Net-SNMP** tools

## 📋 Quick Start
1.  **Clone the repo:**
    ```bash
    git clone https://github.com/mikeosude/unifi-snmp-metrics.git
    ```
2.  **Verify OIDs:** Check the `oids.txt` file for the mapping of your device's specific OIDs.
3.  **Configure Exporter:** Integrate these OIDs into your `snmp.yml` file for the Prometheus SNMP Exporter.
4.  **Visualize:** Import your metrics into your Grafana dashboard.

## 🤝 Contributing
Found a new OID? Have a different UniFi device model? I’d love to include your findings. Please fork this repo and submit a Pull Request!

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

***

### Pro-Tips for your `README.md`:
* **Add a Screenshot:** If you have a Grafana dashboard showing these metrics, take a screenshot of it and add it to a `/images` folder in your repo. Add `![Dashboard Snapshot](images/dashboard.png)` to the README. It’s the single most effective way to make people star your repo.
* **Be Specific:** In the "Quick Start" section, if you have a sample `snmp.yml` configuration snippet, include it in a code block. Users love "copy-paste-ready" documentation.
* **Badges:** You can use [Shields.io](https://shields.io/) to add more badges (like your programming language or tool versions) to make the header look more professional.
