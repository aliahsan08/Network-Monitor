Network Monitor Assignment

Compilation:
make

Running:
sudo ./network_monitor

Requirements:
- Linux system
- Root privileges for raw socket access
- Network interface (default: eth0)

Features:
- Continuous packet capture
- Packet dissection for Ethernet, IPv4, IPv6, TCP, UDP
- Packet filtering by source/destination IP
- Packet replay with delay estimation
- Error handling with retry mechanism
- Backup queue for failed packets

Test Cases:
- Captures packets for 1 minute
- Dissects packets continuously
- Filters packets between specific IPs
- Replays filtered packets
- Handles errors and uses backup queue
