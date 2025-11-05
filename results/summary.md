# Performance Test Summary

## Test Overview
Testing was conducted using **MyOrbit Telkomsel** connection (dynamic IP with CGNAT) to evaluate upload, download, and remote access performance.

| Test Case | File Size | Upload Speed | Download Speed | Access Result | Notes |
|------------|------------|---------------|----------------|----------------|--------|
| Local Network | 10 MB | 8.1 Mbps | 15.2 Mbps | ✅ Successful | Stable connection |
| Local Network | 100 MB | 7.6 Mbps | 13.8 Mbps | ✅ Successful | Minor latency observed |
| Remote via DuckDNS | 10 MB | 5.4 Mbps | 12.3 Mbps | ✅ Successful | Encrypted via SWAG |
| Remote via DuckDNS | 50 MB | 5.2 Mbps | 11.9 Mbps | ✅ Successful | Minor upload delay |
| Remote via Mobile Data | 10 MB | 5.0 Mbps | 10.5 Mbps | ✅ Successful | Slight fluctuation |

## Summary
- **All access modes (local, remote, mobile)** were functional and stable.  
- DDNS and HTTPS integration via SWAG ensured secure external connections.  
- Performance remained within acceptable range for small to medium file operations.

## Observation
This setup is ideal for small organizations that require:
- Controlled data storage ownership  
- Secure web-based access (Nextcloud)  
- Cost-efficient operation with existing hardware
