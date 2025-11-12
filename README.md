# PythonNetworkLogger
Python firewall script that captures network traffic and writes logs to a file. It uses Scapy for packet sniffing and allows you to define simple filtering rules.

Requirements:
Ubuntu 24.04
Scapy - pip install scapy

How It Works
Packet Capture: Uses scapy.sniff() to capture packets in real time.
Filtering Rules: Blocks packets from certain IPs or ports.
Logging: Writes timestamped logs to network_traffic.log with action (ALLOWED or BLOCKED).

sudo python firewall.py
This is a basic type of firewall logger — it monitors and logs but does not actively drop packets at the OS level.
If you want actual packet blocking, you’d need to integrate with iptables (Linux) or netsh (Windows).
