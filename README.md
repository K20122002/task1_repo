# task1_repo
Nmap scan outputs for Task 1
TASK 1 — NMAP & WIRESHARK RESULTS
Date: 22/09/2025
Author: KANISHGA

1) Summary
- Network scanned: [ 10.183.72.36]
- Purpose: Discover open ports on devices in my local/home network and collect packet evidence.

2) Commands I ran (copy-paste exactly what you used)
- Example: nmap  10.183.72.36 -oN nmap-scan.txt
- Example: sudo nmap -sS -p- -T4 -sV  10.183.72.36 -oA task1_scan

 3) Key findings (one short line per host)
- 192.168.x.x — HOSTNAME (if known) — OPEN PORTS: 22/tcp (ssh), 80/tcp (http)
- 192.168.y.y — HOSTNAME — OPEN PORTS: 23/tcp (telnet)  <-- (example)

4) Screenshots & files included (exact filenames)
- screenshots/1_nmap.png  — Terminal showing Nmap scan results
- screenshots/2_wireshark_syn.png — Wireshark capture showing SYN packet
- screenshots/3_wireshark_synack.png — Wireshark capture showing SYN/ACK reply
- nmap_output/nmap-scan.txt — raw Nmap text output
- report.pdf — short summary report

5) How I captured evidence
- I ran Nmap from my PC and saved the output as nmap-scan.txt.
- While scanning, I captured packets using Wireshark and saved the capture as scan_capture.pcapng.
- I took screenshots of terminal and Wireshark windows and saved them in screenshots/.

6) Quick interpretation (one-line conclusions)
- SYN -> SYN/ACK observed for  10.183.72.36:22 indicates port 22 is open (service: SSH).
- RST observed for  10.183.72.36:445 indicates port 445 is closed or blocked.

7) Recommendations
- Close or disable unused services (e.g., Telnet) or restrict access to trusted IPs.
- Patch services/OS and change default credentials.
- Use firewall rules to block unnecessary ports from WAN.

8) Ethics & scope
- I scanned only my own/home network and devices I own or have permission to test.
- No sensitive data (passwords, personal info) is included in uploaded files.

9) Contact / notes
- If reviewer needs raw pcap or additional details, contact: Kanishga2012002@gmail.com

END OF README
