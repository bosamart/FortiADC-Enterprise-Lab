# FortiADC Enterprise Lab

## Overview

Enterprise Layer 7 Application Delivery Lab built using:

- FortiADC 7.4.4
- FortiGate
- Cisco NXOS
- Ubuntu Linux
- Apache2

This lab demonstrates:

- Layer 7 Load Balancing
- HTTPS Offloading
- Persistence (Sticky Session)
- OSPF Routing
- Content Routing
- Health Checks
- Multi-tier Application Architecture

---

## Topology

Client
→ FortiGate
→ FortiADC
→ Backend Application Servers

---

## Backend Servers

| Server | Role | IP |
|---|---|---|
| WEB-FRONTEND-01 | Frontend Website | 192.168.102.12 |
| API-SRV-01 | API Service | 192.168.102.13 |
| STATIC-CONTENT-01 | Static Content | 192.168.102.14 |

---

## Content Routing

| URL | Destination Pool |
|---|---|
| / | FRONTEND_POOL |
| /api | API_POOL |
| /images | STATIC_POOL |

---

## Technologies Used

- FortiADC
- FortiGate
- Cisco NXOS
- Apache2
- OSPF
- HTTPS
- Layer 7 ADC
