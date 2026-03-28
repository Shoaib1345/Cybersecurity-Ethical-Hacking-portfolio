## 📌 Project Overview

Delivered as a freelance project for a university cybersecurity module client.

A 4-lab hands-on security portfolio covering offensive techniques,
vulnerability assessment methodology, and professional reporting —
conducted in a controlled VirtualBox environment using Kali Linux.

**Client:** University cybersecurity student (CMP-X305 module)
**Delivered:** March 2026
**Tools:** Kali Linux · WPScan · OWASP Juice Shop · Nessus Essentials ·
tcpdump · VirtualBox · rockyou.txt

## ⚠️ Challenges & Solutions

### 1. VM Network Connectivity
**Problem:** VMs couldn't communicate — adapters not on the same Internal Network.
**Solution:** Configured both VMs to Internal Network mode with static IPs
in the 192.168.123.x subnet. Verified with bidirectional ping at 0.5ms.

### 2. Client-Side Control Bypass (Juice Shop)
**Problem:** Disabled submit button appeared to block form submission.
**Solution:** Removed 'disabled' attribute via browser dev tools — form submitted.
**Lesson:** Client-side controls are never a security boundary.

### 3. Nessus Plugin Compilation
**Problem:** Nessus unusable immediately after install — plugins not ready.
**Solution:** Allowed 15–30 min compilation to complete before scanning.

### 4. WPScan Brute Force Configuration
**Problem:** Needed to correctly target the right user and wordlist.
**Solution:** Used --enumerate u flag first, then passed rockyou.txt
via --passwords — cracked weak password '123456' within seconds.
