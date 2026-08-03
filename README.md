# PCAP Incident Investigation

![](screenshots/pcap-incident-investigation.png)

## Overview

_Investigation based on a public malware dataset published by malware-traffic-analysis.net._

This project documents a network investigation performed on a PCAP capture related to a suspected malware infection.

The objective was to identify suspicious network activity, analyze malicious communications, extract indicators of compromise (IOCs), enrich findings with threat intelligence, and create detection rules.

## Investigation Workflow

The analysis followed these steps:

1. Case information and investigation scope
2. PCAP triage and traffic overview
3. Network deep dive:
   - DNS analysis
   - HTTP analysis
   - File extraction
   - Communication analysis
4. Threat intelligence enrichment
5. Impact assessment
6. Final report and detection rules

## Key Findings

The investigation identified:

- Malicious document delivery (`Doc3134.doc`)
- Malicious executable delivery (`rFrUanXYL.exe`)
- Communications with suspicious external infrastructure
- Multiple indicators of compromise including:
  - Domains
  - IP addresses
  - File hashes

## Tools Used

- Wireshark
- capinfos
- VirusTotal
- Suricata

## Repository Structure


```
PCAP-Incident-Investigation/
├── README.md
│
├── 01_CASE_INFORMATION/
│   └── case_information.md
│
├── 02_TRIAGE/
│   └── triage_notes.md
│
├── 03_DEEP_DIVE/
│   ├── deep_dive_analysis.md
│
├── 04_THREAT_INTEL/
│   ├── IOC_table.md
│   └── mitre_attack_mapping.md
│
├── 05_IMPACT_ASSESSMENT/
│   └── impact_assessment.md
│
├── 06_FINAL_REPORT/
│   ├── final_report.md
│   └── detection_rules/
│      └── suricata.md
│
└── screenshots/
```

## Disclaimer

This investigation is based only on network evidence available in the PCAP capture.

File execution, persistence mechanisms, and post-compromise activity cannot be confirmed without additional endpoint analysis.
