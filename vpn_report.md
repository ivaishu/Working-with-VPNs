# VPN Setup & Test Report – Surfshark VPN (Windows 11)

## Objective
Understand and demonstrate how a VPN works for privacy and security by:
- Connecting to a VPN
- Verifying IP change
- Checking encryption
- Recording observations

---

## Step-by-Step Process

### Step 1: Connect to VPN
- Launched **Surfshark VPN** on Windows 11.
- Logged in with my account.
- Selected server location: **Germany**.
- Connection successful (see `vpn-connected.png`).

### Step 2: Verify IP Change
- **Before VPN**: My real IP was detected via [whatismyipaddress.com] – blurred for privacy in `ip-before.png`.
- **After VPN**: The IP changed to VPN server’s IP in the chosen country (`ip-after.png`).

### Step 3: Check Encryption (ipleak.net)
- Visited [ipleak.net] while connected to VPN.
- **Findings:**
  - IPv4 address shown: VPN server IP only (no real IP visible).
  - IPv6: Not detected (VPN blocking IPv6).
  - DNS servers: All routed through VPN, no DNS leak.
  - WebRTC IP: Matches VPN IP, no local IP exposed.
  - Connection encrypted with AES-256 via OpenVPN protocol.
- See `encryption-test.png` for blurred screenshot.

### Step 4: Compare Speed
- Ran [fast.com](https://fast.com) before and after VPN connection.
- Observed a speed drop from **45 Mbps** to **33 Mbps** (download) due to encryption overhead.
- Screenshots: `speed-test-before.png` (before VPN) and `speed-test-after.png` (after VPN).

---

## Findings

| Aspect Tested         | Result |
|-----------------------|--------|
| IP Address Changed    | ✅ Yes |
| IPv6 Leaks            | ❌ None |
| DNS Leaks             | ❌ None |
| WebRTC Leak           | ❌ None |
| Traffic Encrypted     | ✅ Yes |
| Speed Impact          | Moderate slowdown |

---

## Benefits of Using Surfshark VPN
1. Hides real IP and location
2. Encrypts internet traffic (AES-256 encryption)
3. Prevents DNS, IPv6, and WebRTC leaks
4. Allows bypassing geo-restrictions
5. No-logs policy for privacy

---

## Limitations
- Reduced internet speed compared to direct connection
- Some streaming services block VPN servers
- Relies on trust in the VPN provider

---

## Conclusion
This exercise demonstrated how Surfshark VPN successfully hides the real IP, encrypts traffic, and prevents leaks through DNS, IPv6, and WebRTC.  
While VPNs add a strong layer of privacy and security, they are not a complete anonymity solution and should be used alongside other security practices.

---

**Screenshots:** See the `/screenshots` folder for all test evidence.
