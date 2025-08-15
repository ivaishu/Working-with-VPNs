# Working-with-VPNs

## Overview
This repository contains the work for my Cyber Security Internship task: **Working with VPNs**.  
Although the original instructions recommended using a free VPN, I have adapted the task to use my existing **Surfshark VPN (Paid Subscription)** on Windows 11.

The objective was to:
- Set up and connect to a VPN
- Verify the IP change
- Confirm encryption
- Summarize VPN benefits and limitations

---

## Steps Followed

### 1. VPN Setup
- Opened **Surfshark VPN** on Windows 11
- Logged in with my account
- Selected a VPN server (Country: **Germany**
- Connected successfully ✅

### 2. IP Verification
- **Before VPN**: Visited [whatismyipaddress.com](https://whatismyipaddress.com) and recorded my real IP *(blurred in screenshots for privacy)*.
- **After VPN**: Verified the IP had changed to the VPN server location.
- See screenshots in [`/screenshots`](./screenshots/).

### 3. Encryption Check
- Verified that traffic was encrypted using [ipleak.net](https://ipleak.net/) and DNS/IP Leak tests.
- Confirmed no DNS or IPv6 leaks.

### Step 4: Compare Speed
- Ran [fast.com](https://fast.com) before and after VPN connection.
- Observed a speed drop from **45 Mbps** to **33 Mbps** (download) due to encryption overhead.
---

## Results Summary
| Test                | Before VPN | After VPN  |
|--------------------|------------|------------|
| IP Address         | Real IP (hidden) | 217.138.216.230 |
| Location Detected  | Thrissur    | Germany |
| Download Speed     | 45 Mbps    | 33 Mbps    |
| Upload Speed       | 46 Mbps    | 34 Mbps    |
| Encryption Status  | Not encrypted | Encrypted |

---

## Benefits of VPN
- Masks real IP address and location
- Encrypts internet traffic to protect from eavesdropping
- Allows bypassing geo-restrictions
- Protects data on public Wi-Fi

## Limitations of VPN
- Possible reduction in internet speed
- VPN provider must be trusted with your traffic
- Some websites may block VPN IP ranges
- Does not make you 100% anonymous

---

## Screenshots
All screenshots are stored in the [`/screenshots`](./screenshots/) folder:
- `vpn-connected.png` – Surfshark connected
- `ip-before.png` – IP before VPN (blurred some digits)
- `ip-after.png` – IP after VPN 
- `encryption-test.png` – Encryption confirmation
- `speed-test-before.png` – Speed test result before VPN connection
- `speed-test-after.png` – Speed test result after VPN connection

---

## References
- [Surfshark VPN](https://surfshark.com/)
- [WhatIsMyIPAddress](https://whatismyipaddress.com)
- [IP Leak Test](https://ipleak.net/)
- [fast.com](https://fast.com)

---
**Note:** IP addresses in the screenshots have been partially blurred for privacy.
