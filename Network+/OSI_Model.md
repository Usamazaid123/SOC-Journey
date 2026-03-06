# OSI Model – SOC Perspective

## Layer 7 – Application
What it does:
Handles user-facing applications and services.

Common attack:
SQL injection, malware delivery.

SOC view:
Monitor web logs, abnormal requests, suspicious payloads.

---

## Layer 6 – Presentation
What it does:
Formats, encrypts, and compresses data.

Common attack:
SSL/TLS downgrade attacks.

SOC view:
Watch encryption issues, certificate warnings.

---

## Layer 5 – Session
What it does:
Manages sessions between systems.

Common attack:
Session hijacking.

SOC view:
Look for abnormal session timeouts or reuse.

---

## Layer 4 – Transport
What it does:
Controls data flow using TCP/UDP.

Common attack:
Port scanning, SYN flood.

SOC view:
Monitor unusual port activity and connection spikes.

---

## Layer 3 – Network
What it does:
Routes packets using IP addresses.

Common attack:
IP spoofing.

SOC view:
Analyze traffic flow and routing anomalies.

---

## Layer 2 – Data Link
What it does:
Handles MAC addressing and local delivery.

Common attack:
ARP spoofing.

SOC view:
Detect ARP anomalies and MAC flooding.

---

## Layer 1 – Physical
What it does:
Physical transmission of data.

Common attack:
Cable unplugging, hardware tampering.

SOC view:
Physical access alerts and outages.



----------
OSI model or OSI reference model is used to categorize the functions of a network, Useful for troubleshooting, operates under tcp/ip model
7- Application - Data 
6- Presentation - Data 
5- Session - Data 
4- Transmission - Segments 
3- Network - Packets 
2- data link - Frames 
1- Physical - Bits 

-------------

Layer 1 – Physical
Purpose
Transmission of bits across the network, using cat5 or 6

*Data:
Binary bits (1s and 0s) 

*Signals:
Copper = voltage 0=0v, 1=+5/-5
Fiber = light 1=light on, 0=lighht off

*Connectors: RJ-45:Ethernet cable connector

*Cable Standards
568A: Ethernet wiring standard -           GBRB - Green, Blue, Red, Black
568B: Alternate Ethernet wiring standard   RBGB - Red, Blue, Green, Black
Crossover cables – TIA/EIA-568A on one end, and TIA/EIA-568B on the other end
Straight-through cables – TIA/EIA-568B on both ends

*Topologies
Bus: Single shared cable
Ring: Devices in circular path
Star: Devices connected to central switch
Mesh: Devices interconnected for redundancy

Asynchronons: sender wait for the reciever(voice note)
Synchronous: use reference clock(on a call )
baseband: Entire bandwidth used by one signal Example: Ethernet
broadband:Bandwidth divided into channels Example: cable TV

*Multiplexing
TDM: Fixed time slots for signals
StatTDM: Dynamic time slot allocation
FDM: Different frequency channels

*infrastructure Devices
Hubs: Repeat signals to all ports
Access points: Provide wireless network access
Media converters: Convert fiber ↔ Ethernet signals

------
Layer 2 – Data Link Layer

Packages bits from Layer 1 into frames and ensures reliable data transfer on the local network.

Data Unit

Frame — structured data packet

*Functions

Framing — bits → frames

MAC addressing — device identification

Error detection — detect corrupted frames

Flow control — control data rate

*MAC Address

48-bit physical address — unique hardware ID

First 24 bits → manufacturer — vendor identifier

Last 24 bits → device — unique device ID

*Devices

NIC — network connection card

Bridge — connect network segments

Switch — intelligent LAN device

Switch

Uses CAM table — MAC-to-port mapping

Forwards frames based on MAC address — targeted frame delivery

