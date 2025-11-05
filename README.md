# Network Attached Storage (NAS) with Port Forwarding and DDNS

Implementation of **Network Attached Storage (NAS)** using **Port Forwarding** and **Dynamic Domain Name Service (DDNS)** as an alternative data storage solution at **PT XYZ**.

## Overview
This project was developed as an undergraduate thesis at Universitas Trisakti.  
The goal was to create a **self-hosted storage system** that can be accessed securely from anywhere, providing a low-cost and efficient alternative to commercial cloud storage.  
The system integrates **OpenMediaVault**, **Nextcloud**, **DuckDNS**, and **Docker** on a **Raspberry Pi** device.

**Objective:**  
To improve accessibility and flexibility of data storage for small-scale organizations without relying on third-party cloud providers.

## Environment & Tools
| Component | Description |
|------------|-------------|
| **Hardware** | Raspberry Pi 4 Model B, HDD 1 TB, Router Huawei B311B |
| **Operating System** | Raspberry Pi OS Lite |
| **Core Software** | OpenMediaVault (OMV), Docker, Nextcloud, Portainer |
| **Support Services** | DuckDNS (for DDNS), SWAG (for HTTPS reverse proxy) |
| **Network** | MyOrbit by Telkomsel (up to 15 Mbps, dynamic IP) |

## Implementation Steps
1. Install **Raspberry Pi OS Lite** and configure SSH access.  
2. Install **OpenMediaVault** using the official script.  
3. Add the **Docker** plugin and set up containers for Nextcloud, MariaDB, Portainer, and SWAG.  
4. Configure **Port Forwarding** on the router to expose required ports.  
5. Register a sub-domain on **DuckDNS** and link it with SWAG for secure external access.  
6. Test accessibility via SSH, OpenMediaVault GUI, and Nextcloud web interface.

## Testing Summary
| Parameter | Method | Result |
|------------|---------|--------|
| **Functionality** | SSH / OMV / Portainer / DDNS / Nextcloud | All accessible and stable |
| **Data Transfer Test** | Upload & Download (10 MB / 50 MB / 100 MB files) | Average upload ≈ 5–8 Mbps, download ≈ 12–15 Mbps |
| **Access Mode** | Local & Remote (via DuckDNS domain) | Successful connection from both desktop & mobile |

## Learning Outcomes
- Implemented a complete **NAS infrastructure** with DDNS and port forwarding.  
- Gained practical experience in **server configuration**, **network routing**, and **remote access management**.  
- Understood performance differences between local and remote data transfer.  
- Applied **incremental development methodology** to minimize configuration risks.  
- Strengthened knowledge in **Linux system administration** and **cloud alternatives**.

## Author
**Annas Al Farisi Riwayadi**  

📧 [annasalfarisi@gmail.com](mailto:annasalfarisi@gmail.com)  
🔗 GitHub [annasalfa](https://github.com/annasalfa)  
💼 LinkedIn [linkedin.com/in/annasalfa](https://linkedin.com/in/annasalfa)

## License
MIT License © 2025 Annas Al Farisi  
Free for personal and educational use with attribution.
