# MITRE ATT&CK Mapping

| Tactic | ATT&CK ID | Technique | Evidence |
|---|---|---|---|
| Initial Access | T1566.001 | Spearphishing Attachment | HTTP response delivered `Doc3134.doc`. |
| Execution | T1204.002 | User Execution: Malicious File | `AutoOpen` macro runs automatically when the document is opened. |
| Execution | T1059.001 | Command and Scripting Interpreter: PowerShell | Decoded macro payload runs a PowerShell download command. |
| Defense Evasion | T1027 | Obfuscated Files or Information | Macro code obfuscated via string fragmentation and reversed strings. |
| Defense Evasion | T1036 | Masquerading | `rFrUanXYL.exe` metadata impersonates a legitimate Microsoft tool. |
| Defense Evasion | T1070.004 | Indicator Removal: File Deletion | `rFrUanXYL.exe` deletes itself after copying to `paramvolume.exe`. |
| Command and Control | T1105 | Ingress Tool Transfer | HTTP response delivered `rFrUanXYL.exe`. |
| Command and Control | T1071.001 | Application Layer Protocol: Web Protocols | Malware communications over HTTP. |
| Command and Control | T1573 | Encrypted Channel | Confirmed by VirusTotal sandbox on the same file hash. |

## Limitations

Network traffic and static/dynamic analysis confirm delivery, execution, 
and evasion behavior. Network activity from the executable itself was not 
observed in the isolated analysis environment; C2 behavior is confirmed 
through external sandbox data (VirusTotal) rather than direct observation.