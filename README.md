# WISP-Network-Setup-and-Troubleshooting
Hands-on networking project focused on WISP configuration, wireless network extension, and real-world troubleshooting.

WISP Router Setup and Network Troubleshooting
Objective

This project documents the process of configuring a TP-Link router to extend and redistribute internet connectivity using WISP mode.
The setup included troubleshooting network routing, DHCP configuration, subnet conflicts, and internet access issues.

Initial Configuration Attempt

At first, the router was configured manually using extender-like settings instead of proper WISP mode.

Manual Configuration
DHCP: Enabled
Router IP: 192.168.0.1
The main router network used a different subnet: 192.168.10.1
Because of the subnet mismatch, the router could not properly communicate with the upstream gateway.

Problem Encountered
Issue 1 — Subnet Conflict

The manually configured router IP was on a different subnet than the main router.

Result
Devices could connect to WiFi
Internet access failed
Gateway communication did not work properly

Issue 2 — DNS Configuration

A manual DNS configuration was attempted using: 8.8.8.8
However, internet connectivity still failed because the main issue was related to gateway and routing configuration rather than DNS resolution.

Solution

The router configuration was changed from manual extender-style setup to proper WISP mode.

WISP Configuration
WISP mode enabled
DHCP enabled
Auto Detect enabled

In WISP mode, the router automatically obtained:

Gateway information
WAN configuration
Routing information from the main router
Important Lessons Learned
Correct subnet configuration is critical in wireless routing.
DNS configuration alone cannot solve routing or gateway issues.
WISP mode simplifies wireless internet redistribution by automatically detecting upstream network settings.
Correct SSID and password configuration are essential for stable wireless connectivity.
Final Result

After enabling WISP mode with automatic detection:

Internet connectivity worked successfully
Client devices received proper DHCP addresses
Wireless redistribution became stable and functional
Technologies / Concepts Used
WISP Mode
DHCP
Gateway Routing
Wireless Networking
DNS Configuration
Subnetting
Network Troubleshooting
