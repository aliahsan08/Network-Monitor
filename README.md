# Network Monitor – Packet Capture, Filtering, and Replay System

## Overview
This project implements a **Network Monitoring System** in **C++** using **raw sockets**.  
It captures, filters, dissects, and replays live network packets in real time using **custom-built data structures** (stack and queue).  
Developed for a Linux environment, it demonstrates how data structures support efficient network traffic management.

---

## Features
- Continuous packet capture via raw sockets  
- Stack-based dissection of Ethernet, IPv4, IPv6, TCP, and UDP layers  
- Packet filtering by source and destination IPs  
- Replay with automatic retry (2 attempts on failure)  
- Backup queue for failed replays  
- Real-time display of packet information  

---

## Requirements
- **C++11 or later**  
- **Root privileges** (for raw socket access)  
- **Linux environment** (native or via VirtualBox)  
- **Make utility** for compilation  

---

## Setup & Execution

### For Linux Users
1. Open a terminal in the project directory.
2. Install the required packages in the terminal.
   ```bash
   sudp apt update
   sudo apt install g++ make build-essential
4. Compile the program:  
   ```bash
   make
5. Run the executable with root privileges
   ```bash
   sudo ./network_monitor

### For Windows Users (via VirtualBox)

1. Install VirtualBox and create a Linux VM (recommended: Ubuntu 22.04).
2. Transfer project files into the VM (e.g. using shared folders or google drive).
3. Install the required packages in the terminal.
   ```bash
   sudp apt update
   sudo apt install g++ make build-essential
4. Inside the VM terminal, navigate to your project files directory:
   ```bash
   cd ~/path-to-your-directory
5. Compile the program:  
   ```bash
   make
6. Run the executable with root privileges
   ```bash
   sudo ./network_monitor

Observe captured packets in the terminal output.

# Author
Ali Ahsan
Data Structures & Algorithms - Assignment 2
National University of Sciences and Technology (NUST)
