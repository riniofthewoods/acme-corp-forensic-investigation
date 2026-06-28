
# Acme Corp Digital Forensic Investigation

## Case Overview
A forensic investigation of a compromised Linux server 
belonging to Acme Corp. The investigation involved mounting 
a DD disk image and analyzing artifacts to reconstruct a 
data breach involving customer financial records.

## Tools Used
- steghide
- zsteg
- binwalk
- John the Ripper
- strings/xxd
- last/lastb
- nginx log analysis
- NAXSI WAF log analysis

## Key Findings
- Identified nginx web server as initial attack surface
- Discovered SQL injection and git credential harvesting attempts
- Identified compromised user account clifford
- Recovered stolen AccountingDB.csv containing customer financial data
- Discovered steganographic PNG disguised as system log (eruces.log)
- Cracked embedded MD5 hash revealing attacker signature
- Attributed attack to threat actor alias sha1337

## Skills Demonstrated
- Digital forensics
- Log analysis
- Steganography detection
- Hash cracking
- Linux forensics
- Incident response
- Threat actor attribution
- Technical report writing

## Attack Timeline
| Date | Event |
|------|-------|
| March 22, 2024 | Attacker creates steganographic PNG |
| March 28, 2024 | AccountingDB.csv stolen and staged |
| April 2, 2024 | Web server reconnaissance and attack |
| April 7, 2024 | Attacker wipes logs and covers tracks |

## Disclaimer
This investigation was conducted in a controlled academic 
environment using a provided forensic disk image. All findings 
are for educational purposes only.
