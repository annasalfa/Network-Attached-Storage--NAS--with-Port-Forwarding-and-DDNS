# Abstract and Overview

## Abstract
This project implements a **Network Attached Storage (NAS)** system utilizing **Port Forwarding** and **Dynamic Domain Name Service (DDNS)** as an alternative data storage solution at **PT. XYZ**.  
The goal is to enable secure and efficient remote access to files without relying on paid cloud services such as Google Drive or Dropbox.

The system was built on a **Raspberry Pi 4 Model B** running **Raspberry Pi OS Lite**, using **OpenMediaVault (OMV)** as the NAS operating system.  
Key supporting tools include **Docker**, **Nextcloud**, **DuckDNS**, **SWAG**, and **Portainer** for container management.

## Objectives
- Provide a low-cost, self-hosted cloud storage solution for small-scale organizations.  
- Enable secure remote access via DDNS and HTTPS configuration.  
- Optimize local and remote data transfer using OpenMediaVault and Nextcloud integration.  
- Demonstrate real-world implementation of NAS deployment on a dynamic IP network.

## System Architecture
The NAS is hosted on a Raspberry Pi 4 with 1 TB HDD storage.  
Access is managed through local IP for intranet users and a DDNS domain for remote users.  
Port Forwarding and SWAG (Secure Web Application Gateway) ensure encrypted connections using HTTPS.

**Components:**
- **OpenMediaVault** — Core NAS system for storage management.  
- **Docker & Portainer** — Container orchestration and service monitoring.  
- **Nextcloud** — Web-based user access for uploads and file synchronization.  
- **DuckDNS** — Dynamic DNS mapping for public domain access.  
- **SWAG** — Reverse proxy with automatic SSL certification.

## Results Summary
The system was successfully deployed and tested under MyOrbit (Telkomsel) network conditions with dynamic IP (CGNAT).  
Testing confirmed stable connections from both local and remote clients via the DuckDNS domain.

Average performance:
- Upload Speed: **5–8 Mbps**
- Download Speed: **12–15 Mbps**
- Access: **Stable from Desktop, Mobile, and Remote Network**

## Conclusion
The NAS implementation effectively replaces commercial cloud solutions for small-scale environments.  
It provides better control over data privacy and scalability, while maintaining reliable access and manageable performance within a constrained network environment.
