peer-to-peer-lan-verification
Cisco Packet Tracer lab for configuring static IPv4 addressing, switch connectivity, ping verification, and ARP resolution between two PCs.


Peer-to-Peer Local Area Network Verification

Experiment Overview

This experiment demonstrates the configuration and verification of a simple Peer-to-Peer Local Area Network (LAN) using two workstations connected through a Cisco 2960 Layer 2 switch.

Both PCs are configured with static IPv4 addresses in the same subnet. Network connectivity is verified using the `ping` command, and IP-to-MAC address resolution is verified using the `arp -a` command.



Objective

The objectives of this experiment are:

- Configure static IPv4 addresses on two workstations.
- Connect two PCs through a Cisco 2960 Layer 2 switch.
- Use Copper Straight-Through cables for physical connectivity.
- Verify IPv4 configuration using the `ipconfig` command.
- Test communication between the two PCs using `ping`.
- Inspect the ARP table using `arp -a`.
- Verify successful Layer 2 and Layer 3 communication.


Tools and Devices Used

Devices

- PC0
- PC1
- Cisco 2960 Series Layer 2 Switch

Cables

- Copper Straight-Through Cable × 2

Software
Cisco Packet Tracer
Network Topology


                         Cisco 2960 Switch
                        ┌──────────────────┐
                        │     Switch0      │
                        │                  │
                        │ Fa0/1     Fa0/2  │
                        └───┬─────────┬────┘
                            │         │
                            │         │
                           Fa0       Fa0
                            │         │
                    ┌───────┘         └───────┐
                    │                         │
             ┌──────────────┐          ┌──────────────┐
             │     PC0      │          │     PC1      │
             │              │          │              │
             │192.168.10.25 │          │192.168.10.26 │
             └──────────────┘          └──────────────┘
