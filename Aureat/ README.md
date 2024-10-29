Aureat Tool Documentation



Overview

Aureat is an advanced Automated Threat Intelligence Aggregator designed for cybersecurity professionals to monitor, detect, and respond to network threats in real time. It combines threat intelligence, malware detection, and anomaly monitoring for devices, IoT devices, and servers within a network. Aureat is developed for use directly from the command line, making it suitable for efficient and streamlined cybersecurity operations.




Installation

Prerequisites

Ensure you have Python 3.8+ installed.

You need a global environment set up on your system for CLI tools.


Download and Install

1. Clone the Aureat repository:

git clone https://github.com/garogenius/aureat.git


2. Navigate to the directory:

cd aureat


3. Move the folder to the global directory:

sudo mv aureat /usr/local/bin/


4. Make the tool executable:

sudo chmod +x /usr/local/bin/aureat



Run the Tool

You can now run Aureat globally without specifying python aureat.py.

To execute the tool, simply type:

aureat <command> [options]



Commands and Flags

Below are the commands and flags available in the Aureat tool, along with their descriptions and usage examples.

Device Management

1. Add a Device to the Monitoring List

aureat --add-device <ip_address> <name> <type>

Description: Adds a device with specified IP address, name, and type (e.g., "IoT", "Server") to the monitoring list.

Example:

aureat --add-device 192.168.1.10 "Camera1" "IoT"



2. Remove a Device from the Monitoring List

aureat --remove-device <ip_address>

Description: Removes a device with the specified IP address from the monitoring list.

Example:

aureat --remove-device 192.168.1.10



3. Remove All Devices

aureat --drop-all

Description: Removes all devices from the monitoring list.



4. List All Monitored Devices

aureat --list-devices

Description: Displays all devices currently on the monitoring list.




Alert and Notification Management

5. Specify Email for Alerts

aureat --add-email <email_address>

Description: Sets up the email address to receive alerts and reports.

Example:

aureat --add-email youremail@example.com



6. Email the Generated Report

aureat --email-report

Description: Sends the generated threat report to the specified email.




Threat Detection and Scanning

7. Start Automatic Threat Detection

aureat --start-auto-detection

Description: Starts automatic threat detection, checking every 10 minutes for new threats.



8. Malware Detection

aureat --detect-malware

Description: Runs a malware detection scan on all monitored devices.



9. Block Specific IP Address

aureat --block-ip <ip_address>

Description: Blocks a specified IP address from accessing the network.

Example:

aureat --block-ip 192.168.1.20



10. Sniff Network Traffic

aureat --sniff <interface>

Description: Starts sniffing network traffic for suspicious or malicious activity.

Example:

aureat --sniff eth0



11. Detect Dangerous Threats

aureat --detect-dg-threats

Description: Identifies dangerous threats within the collected threat data.



12. Scan a Device for Vulnerabilities

aureat --scan-device <device_name>

Description: Scans the specified device for known vulnerabilities.

Example:

aureat --scan-device Camera1



13. Scan the Network for Devices and Vulnerabilities

aureat --scan-network

Description: Scans the local network to identify connected devices and assesses their vulnerabilities.



14. Search for Devices

aureat --search-devices

Description: Searches the network for devices like mobile phones, IoT devices, traffic systems, and Bluetooth-enabled devices.




Threat Intelligence and Reporting

15. Fetch Latest Threat Data

aureat --fetch

Description: Retrieves the latest threat data from available threat intelligence feeds.



16. Correlate Threat Data

aureat --correlate

Description: Correlates the fetched threat data with monitored devices to detect potential threats.



17. Generate Threat Report

aureat --report

Description: Generates a detailed threat report for all monitored devices.



18. Open Documentation

aureat --open-doc

Description: Opens the Aureat documentation in the default web browser.



19. Send Feedback

aureat --feedback <title> <content>

Description: Allows you to send feedback directly from the tool interface.

Example:

aureat --feedback "UI Feedback" "Add a graphical interface"




Version

20. Show Tool Version

aureat --version

Description: Displays the current version of the Aureat tool.





Usage Examples

1. Add and Scan a Device

aureat --add-device 192.168.1.10 "Router" "Network Device"
aureat --scan-device Router


2. Start Auto-Detection and Sniffing

aureat --start-auto-detection
aureat --sniff eth0


3. Generate and Email a Threat Report

aureat --report
aureat --email-report




Problem and Solution

Problem: Cybersecurity professionals face the challenge of real-time monitoring, threat detection, and device vulnerability assessment. They need a streamlined, CLI-based tool that aggregates threat intelligence and automates detection across a network.

Solution: Aureat simplifies this process by integrating threat intelligence gathering, device monitoring, malware detection, and network sniffing into a single command-line tool. With Aureat, professionals can stay ahead of threats, automate vulnerability scans, and receive immediate alerts to ensure network safety.
