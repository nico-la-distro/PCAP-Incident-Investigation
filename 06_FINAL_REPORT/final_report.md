## Summary

A network investigation was performed on a PCAP capture from internal host `10.9.4.103`.
The analysis identified malicious file downloads and communications with external infrastructure associated with malicious domains and IP addresses.

## Findings

### Malicious File Delivery

- `Doc3134.doc` was delivered from `devbyjr.com`.
- `rFrUanXYL.exe` was delivered from `boloshortolandia.com`.
- Both files were identified as malicious by VirusTotal.

### External Communications

- Communications with identified suspicious infrastructure were observed:
  - `192.241.188.55`
  - `93.189.41.44`
  - `201.146.211.106`

### Impact

**Confirmed:**
- Malicious files were transferred to the internal host.
- Communication with suspicious external infrastructure occurred.

**Not confirmed:**
- File execution.
- Persistence mechanisms.
- Data theft.
- Lateral movement.

## Recommendations

- Isolate and investigate the affected host.
- Perform endpoint analysis to determine whether downloaded files were executed.
- Block identified domains, IP addresses and file hashes.
- Review logs for additional affected systems.