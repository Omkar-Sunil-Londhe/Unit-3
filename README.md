# NPC – Unit 3 : Configure a DNS Server and Web Server Using Cisco Packet Tracer

Practical assignment for the **Networking Protocols & Communication (NPC)** course.

| | |
|---|---|
| **Student** | Omkar Sunil Londhe |
| **PRN** | 2125UCSM1074 |
| **Department** | Cyber Security |
| **Semester** | 3rd Semester (Second Year) |
| **Subject** | NPC – Unit 3 |
| **College** | Sanjivani University, Kopargaon |
| **Repository** | [https://github.com/Omkar-Sunil-Londhe/Unit-3.git](https://github.com/Omkar-Sunil-Londhe/Unit-3.git) |

## Overview

A single LAN (`192.168.1.0/24`) is built in Cisco Packet Tracer with two PCs, a
Layer-2 switch, a DNS server and a web server. The web server hosts a simple page
over HTTP, and the DNS server resolves the domain **www.npcunit3.com** to the web
server so the site can be opened by name instead of by IP address.

## IP Addressing

| Device | IP Address | Subnet Mask |
|---|---|---|
| DNS Server | 192.168.1.2 | 255.255.255.0 |
| Web Server | 192.168.1.3 | 255.255.255.0 |
| PC0 | 192.168.1.10 | 255.255.255.0 |
| PC1 | 192.168.1.11 | 255.255.255.0 |

- DNS server configured on the PCs: `192.168.1.2`
- DNS A record: `www.npcunit3.com` → `192.168.1.3`
- Default gateway: not required (single subnet)

## Result

Both ping tests (to `192.168.1.2` and `192.168.1.3`) returned 4/4 replies with 0%
packet loss, and the website opened successfully on PC0 via
`http://www.npcunit3.com`, confirming that DNS name resolution and HTTP access work.

## Files
 
| File | Description |
|---|---|
| `NPC_Unit_3_Omkar_Londhe.pdf` | Full practical report in PDF format (submission copy) |
| `NPC_Unit_3_DNS_Web_Server_Report.docx` | Full practical report in editable Word DOCX format |
| `NPC_Unit_3_DNS_Web_Server.pkt` | Cisco Packet Tracer project file |
| `screenshots/` | Real Packet Tracer screenshots (topology, ping, website, simulation) |
| `build_pdf.py` | Script used to generate the PDF report |
| `logical_topology.png` | Logical topology diagram used in the report |
 
> The images in `screenshots/` are genuine captures from Cisco Packet Tracer 9.0.1.

## GitHub Clone Command

```bash
git clone https://github.com/Omkar-Sunil-Londhe/Unit-3.git
```
