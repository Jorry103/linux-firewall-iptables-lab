
# Linux Firewall Configuration and Testing Using iptables

## Overview
This project demonstrates the configuration and testing of a Linux firewall using iptables on Kali Linux.
The objective was to control network traffic by allowing specific services, blocking unauthorized connections, and verifying firewall behavior through practical testing.

## Tools and Technologies
- Kali Linux
- Linux iptables
- Oracle VirtualBox
- Windows PowerShell
- SSH and HTTP
- TCP/IP Networking

## Lab Implementation

### 1. Initial Configuration
- Inspected existing firewall rules.
- Identified the Kali Linux IP address.
- Started SSH and HTTP services.
- Verified network connectivity before applying firewall restrictions.

### 2. Firewall Configuration
- Allowed incoming SSH traffic on TCP port 22.
- Allowed incoming HTTP traffic on TCP port 80.
- Allowed outgoing TCP traffic.
- Allowed loopback and established connections.
- Applied default DROP policies to INPUT, OUTPUT, and FORWARD.

### 3. Firewall Testing
- Verified successful SSH connectivity after applying firewall rules.
- Confirmed HTTP access using an HTTP 200 OK response.
- Demonstrated TCP port 23 blocking through connection testing and firewall packet counters.

### 4. Firewall Cleanup
- Restored default policies to ACCEPT.
- Flushed firewall rules.
- Verified the final firewall configuration.
- Closed test sessions and stopped temporary services.

## Test Results

| Test | Expected Result | Observed Result |
|------|-----------------|-----------------|
| SSH (Port 22) | Allowed | Successful |
| HTTP (Port 80) | Allowed | HTTP 200 OK |
| TCP Port 23 | Blocked | Request timed out; DROP counter increased |
| Firewall Cleanup | Rules removed | Successful |

## Key Skills Demonstrated
- Linux Firewall Administration
- Network Security
- iptables Configuration
- Traffic Filtering
- Network Connectivity Testing
- Firewall Troubleshooting

## Project Report
[View Full Lab Report](Network%20Security%20.pdf)

## Note
This project was implemented in a virtual lab environment for educational purposes.


