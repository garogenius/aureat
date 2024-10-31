

Aureat: Automated Threat Intelligence Aggregator


Aureat is an advanced Automated Threat Intelligence Aggregator, designed to help cybersecurity professionals monitor, detect, and respond to threats across a network. Aureat integrates threat intelligence, device monitoring, malware detection, and vulnerability scanning into a single command-line interface, providing real-time alerts and a streamlined way to protect your digital assets.



Table of Contents

Features

Installation

Commands & Flags

Usage Examples

Contributing

License

https://youtu.be/LThRRkDpiPI?si=lL3Y92596ADFgQyW

https://youtu.be/ZDNCHnmtyAA?si=euORMdLMBpftW9BH

---

Features

Device Management: Easily add, remove, and list devices within your network for monitoring.

Automated Threat Detection: Continuous monitoring and real-time alerts every 10 minutes.

Threat Intelligence Correlation: Fetch and correlate the latest threat data with monitored devices.

Malware & Vulnerability Scanning: Detect malware and scan devices or the entire network for vulnerabilities.

Customizable Alerts: Receive email alerts for immediate threat responses.

Device Search: Identify devices on your network, including IoT, mobile, traffic systems, and Bluetooth devices.



---

Installation

Prerequisites

Python 3.8 or higher.


Steps

1. Clone the Repository

git clone https://github.com/garogenius/aureat.git
cd aureat


2. Move the Tool to Global Directory

sudo mv aureat /usr/local/bin/
sudo chmod +x /usr/local/bin/aureat


3. Run the Tool

Example:

aureat --version





---

Commands & Flags

Below is a list of available commands and flags:

Device Management

--add-device <ip_address> <name> <type>: Add a device to the monitoring list.

--remove-device <ip_address>: Remove a device from the monitoring list.

--drop-all: Clear all devices from the monitoring list.

--list-devices: Display all monitored devices.


Alert and Notification

--add-email <email_address>: Set up the email to receive alerts.

--email-report: Email the generated report.


Threat Detection and Scanning

--start-auto-detection: Begin automatic threat detection every 10 minutes.

--detect-malware: Run malware detection across monitored devices.

--block-ip <ip_address>: Block a specified IP from accessing the network.

--sniff <interface>: Monitor network traffic for suspicious activity.

--detect-dg-threats: Identify dangerous threats within collected threat data.

--scan-device <device_name>: Scan a device for vulnerabilities.

--scan-network: Scan the network for devices and vulnerabilities.

--search-devices: Search for IoT devices, mobile, traffic systems, and Bluetooth devices within the network.


Threat Intelligence and Reporting

--fetch: Fetch the latest threat data.

--correlate: Correlate threat data with monitored devices.

--report: Generate a detailed threat report.

--open-doc: Open the documentation in the browser.

--feedback <title> <content>: Send feedback for tool improvements.


Other Commands

--version: Display the current version of Aureat.



---

Usage Examples

1. Add and Monitor a Device

aureat --add-device 192.168.1.10 "Router" "Network Device"
aureat --scan-device Router


2. Run Automatic Detection and Sniff Network Traffic

aureat --start-auto-detection
aureat --sniff eth0


3. Generate and Email a Threat Report

aureat --report
aureat --email-report


4. Fetch and Correlate Threat Data

aureat --fetch
aureat --correlate




---

Contributing

Contributions are welcome! Please open an issue or submit a pull request to suggest changes, add new features, or fix bugs.

1. Fork the Repository


2. Create a New Branch


3. Make and Commit Your Changes


4. Push to Your Branch


5. Open a Pull Request




---

License

This project is licensed under the MIT License. See the LICENSE file for more information.

<iframe width="560" height="315" src="https://www.youtube.com/embed/LThRRkDpiPI?si=lL3Y92596ADFgQyW" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


---

For questions or feedback, feel free to open an issue or contact us at aureat.tool@gmail.com.


---

