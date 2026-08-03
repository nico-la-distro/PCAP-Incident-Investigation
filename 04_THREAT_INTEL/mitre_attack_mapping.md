| Tactic              | ATT&CK ID | Technique                                 | Evidence                                 |
| ------------------- | --------- | ----------------------------------------- | ---------------------------------------- |
| Initial Access      | T1566.001 | Spearphishing Attachment                  | HTTP response delivered `Doc3134.doc`.   |
| Command and Control | T1105     | Ingress Tool Transfer                     | HTTP response delivered `rFrUanXYL.exe`. |
| Command and Control | T1071.001 | Application Layer Protocol: Web Protocols | Malware communications over HTTP.        |

## Limitations

The PCAP provides evidence of malicious file delivery and external communications. 
Execution of the downloaded files, persistence mechanisms and post-compromise actions cannot be confirmed from network traffic alone.