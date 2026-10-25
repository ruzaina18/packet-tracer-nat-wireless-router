# Packet Tracer Lab: Examine NAT on a Wireless Router

## Overview

This lab demonstrates Network Address Translation (NAT) using a wireless router in Cisco Packet Tracer. Four PCs are configured to obtain private IP addresses through DHCP, and simulated HTTP traffic is examined as it travels from the internal network to an external web server.

## Objectives

- Examine the router's Internet and local network configuration.
- Identify private and public IP addresses.
- Configure four PCs to obtain IP addresses through DHCP.
- Observe HTTP traffic in Simulation mode.
- Compare packet headers before and after NAT translation.

## Tools Used

- Cisco Packet Tracer
- Wireless router
- Four PCs
- DHCP
- NAT
- HTTP
- Simulation mode

## Procedure

### 1. Examine the Internet Connection

- Connected a PC to the wireless router.
- Enabled DHCP on the PC.
- Recorded the default gateway.
- Accessed the router's web-based configuration page.
- Inspected the Internet connection settings under Status > Router.

### 2. Examine the Internal Network

- Opened Status > Local Network.
- Examined the router's local IP address.
- Inspected the DHCP server configuration and address range.
- Identified the private IP addressing used by internal clients.

### 3. Connect Four PCs

- Connected four PCs to the wireless router using straight-through Ethernet cables.
- Enabled DHCP on each PC.
- Used `ipconfig /all` to inspect the assigned IP addresses and network configuration.

### 4. Generate HTTP Traffic

- Switched Packet Tracer to Simulation mode.
- Configured the event filters to display TCP and HTTP traffic.
- Created a Complex PDU using HTTP.
- Selected a PC as the source and the `ciscolearn.nat.com` server as the destination.
- Set the source port to 1000 and configured periodic traffic at 120-second intervals.
- Played the simulation to observe packet movement through the network.

### 5. Examine NAT Translation

- Opened packet events in the Simulation Panel.
- Examined Inbound PDU Details and Outbound PDU Details.
- Compared source and destination IP addresses.
- Observed the source IP address change as the packet passed through the router.

## Key Learnings

- Difference between private and public IP addresses.
- Role of DHCP in assigning IP addresses automatically.
- Purpose of NAT in allowing internal devices to communicate with external networks.
- How HTTP traffic uses TCP.
- How to inspect packet headers using Cisco Packet Tracer Simulation mode.

## Results

The lab was performed in Cisco Packet Tracer to examine NAT configuration and observe simulated HTTP traffic across a wireless router.

Add the actual IP addresses and packet-header observations from the completed simulation to document the results accurately.

## Cybersecurity Relevance

Understanding NAT and packet headers helps with network troubleshooting, traffic analysis, and understanding how internal devices communicate with external servers.

## Screenshots

Add screenshots showing:

1. Router Internet connection status.
2. Local network and DHCP configuration.
3. IP configuration of the four PCs.
4. HTTP traffic in Simulation mode.
5. Inbound and outbound PDU details showing NAT translation.

## Conclusion

This lab provided hands-on experience examining NAT, private IP addressing, DHCP, and HTTP packet flow in a simulated network environment.

**Environment:** Cisco Packet Tracer  
**Project Type:** Networking and Cybersecurity Fundamentals
