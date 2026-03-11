# Hashcat
```Password-cracking tool widely used in security testing```
## Installation & Setup
### Debian/Ubuntu:
### MacOS:
### Using Docker
### From Source:

### Real Pentesting Attack Scenerios
```
hashcat -m 1000 hashes.txt rockyou.txt               #Crack NTLM hashes from a Windows dump
hashcat -m 5600 netntlmv2.txt rockyou.txt            #Crack captured NetNTLMv2 hashes
hashcat -m 18200 asrep_hashes.txt rockyou.txt        #Crack AS-REP roasted Kerberos hashes
hashcat -m 13100 kerberoast_hashes.txt rockyou.txt   #Crack Kerberoasted service tickets
hashcat -m 2100 dcc_hashes.txt rockyou.txt           #Crack Domain Cached Credentials (DCC2)
hashcat -m 7500 wifi.hccapx rockyou.txt              #Crack WPA/WPA2 handshake
hashcat -m 11600 7zip.hash rockyou.txt               #Crack 7zip encrypted archive
hashcat -m 13600 keepass.hash rockyou.txt            #Crack KeePass database password
hashcat -m 9600 office.hash rockyou.txt              #Crack MS Office document password
hashcat -m 10500 pdf.hash rockyou.txt                #Crack PDF password
```


