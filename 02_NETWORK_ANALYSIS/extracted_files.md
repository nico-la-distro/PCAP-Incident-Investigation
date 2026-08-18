# Extracted Files
## Metadata

**source** : Wireshark → Export Objects → HTTP

**Objective:**

Document metadata of files extracted from HTTP traffic, prior to malware analysis.

### Extracted Files

```powershell
Get-FileHash .\Payments -Algorithm SHA256
Get-FileHash .\ozylgj6Z6 -Algorithm SHA256
```

| File Name | SHA256                                                           |
| --------- | ---------------------------------------------------------------- |
| Payments  | FB984E86DD6A8018A58DFF37C13B3AA2B157025C6F11DE5249A101DA10CEEB90 |
| ozylgj6Z6 | 80BCA6CEC3F235547C36C5CF8DA9DFAE6A1F3C4DA71DEA4DCF40EAC342E293C3 |

```bash
file Payments
file ozylgj6Z6
```

| File Name | File Type                           | Reported Filename |
| --------- | ----------------------------------- | ----------------- |
| Payments  | Composite Document File V2 Document | Doc3134.doc       |
| ozylgj6Z6 | PE32 executable (GUI) Intel 80386   | rFrUanXYL.exe     |

### Observations

- Two files were successfully extracted from HTTP responses.
- One file is identified as a Microsoft Word document.
- One file is identified as a Windows PE32 executable.
- File hashes were collected for further reputation analysis.


