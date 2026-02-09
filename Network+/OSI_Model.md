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
