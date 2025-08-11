# Capture and Analyze Network Traffic Using Wireshark

## Objective
Capture live network packets using Wireshark, identify protocols in the traffic, and produce both a `.pcapng` file and a detailed report.

## Tools Used
- Wireshark (Free & Open Source)
- OS: Windows 10
- Browser: Microsoft Edge / Chrome (used to generate traffic)

## Repository Structure
- README.md # Main project overview (this file)
- REPORT.md # Detailed protocol analysis from the capture
- capture.pcapng # Packet capture file

## Steps Performed
1. Installed and opened Wireshark.
2. Selected the active network interface (Wi-Fi).
3. Started capture.
4. Generated network activity:
   - Visited multiple websites.
   - Performed a `ping google.com, ping Microsoft.com, ping Bing.com` in Command Prompt.
5. Stopped capture after ~1 minute.
6. Viewed **Statistics → Protocol Hierarchy** to identify protocols.
7. Saved file as `capture.pcapng`.
8. Created `REPORT.md` for detailed analysis.

## Summary of Findings
- Protocols observed: QUIC (HTTP/3), TCP, TLS, DNS, mDNS, ICMP, ARP.
- QUIC traffic dominated the capture, showing modern encrypted HTTP/3 activity.
- TLS traffic indicates secure HTTPS sessions.
- DNS lookups were present for website resolutions.
- ICMP packets from ping test.
- ARP for local device discovery.

## How to View the Capture
1. Install Wireshark.
2. Open `capture.pcapng`.
3. Use the filter bar to view specific traffic types (e.g., `quic`, `tcp`, `tls`, `dns`).

