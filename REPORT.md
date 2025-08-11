# Wireshark Network Traffic Analysis

## Objective
Capture live network packets and identify different protocols and traffic types.

## Capture Details
- **Date of Capture:** 2025-08-11
- **Duration:** ~1 minute
- **Total Packets:** 16,263
- **File Name:** capture.pcapng

## Protocol Breakdown
| Protocol | % Packets | Packets | % Bytes | Bytes |
|----------|-----------|---------|---------|-------|
| QUIC IETF | 49.2% | 8007 | 52.7% | 5,985,895 |
| TCP | 46.1% | 7504 | 1.4% | 154,700 |
| TLS | 11.7% | 1901 | 40.0% | 4,547,942 |
| DNS | 2.9% | 465 | 0.3% | 34,862 |
| MDNS | 0.3% | 43 | 0.1% | 11,654 |
| ICMP | 0.2% | 33 | 0.0% | 1,420 |
| ARP | 0.5% | 74 | 0.0% | 2,072 |

## Observations
- **QUIC (HTTP/3)** accounted for almost half of all packets, indicating modern encrypted web traffic usage.
- **TCP + TLS** traffic shows encrypted HTTPS sessions.
- **DNS** and **mDNS** traffic confirm active domain resolution for websites and local network services.
- **ICMP** packets were generated during ping tests.
- **ARP** activity indicates standard local network device discovery.

## Conclusion
The capture reflects a typical secure browsing session with significant QUIC traffic, domain lookups, and local network protocol exchanges.
