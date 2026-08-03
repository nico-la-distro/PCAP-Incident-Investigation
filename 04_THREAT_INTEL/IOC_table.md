## File Hashes

**source** : VirusTotal

| IOC | Type | Detection | Notes |
|---|---|---|---|
| FB984E86DD6A8018A58DFF37C13B3AA2B157025C6F11DE5249A101DA10CEEB90 | SHA256 | Trojan 46/63 | Payments / Doc3134.doc |
| 80BCA6CEC3F235547C36C5CF8DA9DFAE6A1F3C4DA71DEA4DCF40EAC342E293C3 | SHA256 | Trojan 57/68 | ozylgj6Z6 / rFrUanXYL.exe |

## Domain Reputation

**source** : VirusTotal

**Lookup date:** 2026-08-03

| IOC | Detection | Notes |
|---|---|---|
| devbyjr.com | 9/91 malicious | Resolved to 66.147.244.86<br>Delivered `Doc3134.doc` |
| boloshortolandia.com | 8/91 malicious | Resolved to 192.241.188.55<br>Delivered `rFrUanXYL.exe` |
| tybalties.website | 8/91 malicious | Resolved multiple times to 93.189.41.44 |

## IP Addresses

**source** : PCAP analysis

| IOC | Type | Notes |
|---|---|---|
| 66.147.244.86 | IPv4 | Associated with devbyjr.com |
| 192.241.188.55 | IPv4 | Associated with boloshortolandia.com, delivered `rFrUanXYL.exe` |
| 93.189.41.44 | IPv4 | Associated with whoulatech.com and tybalties.website, WebSocket traffic observed |
| 201.146.211.106 | IPv4 | HTTP communication observed on port 7080 |
