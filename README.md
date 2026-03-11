# Hashcat
password-cracking tool widely used in security testing
## Installation & Setup
### Debian/Ubuntu:
```sudo apt update && sudo apt install hashcat```
### MacOS:
```brew install hashcat```

### Using Docker
```docker pull hashcat/hashcat ```
```docker run -it --rm hashcat/hashcat --help```

### From Source:
```
git clone https://github.com/hashcat/hashcat.git
cd hashcat
make
./hashcat --help
```

# Hashcat Hash Modes
```
hashcat -m 0 hashes.txt wordlist.txt                       #MD5 Hash
hashcat -m 100 hashes.txt wordlist.txt                     #SHA1
hashcat -m 1400 hashes.txt wordlist.txt                    #SHA256
hashcat -m 1700 hashes.txt wordlist.txt                    #SHA512
hashcat -m 500 hashes.txt wordlist.txt                     #md5crypt
hashcat -m 1500 hashes.txt wordlist.txt                    #descrypt (DES Unix)
hashcat -m 1800 hashes.txt wordlist.txt                    #sha512crypt (Unix)
hashcat -m 3200 hashes.txt wordlist.txt                    #bcrypt
hashcat -m 1000 hashes.txt wordlist.txt                    #NTLM Hash
hashcat -m 3000 hashes.txt wordlist.txt                    #LM Hash
hashcat -m 5500 hashes.txt wordlist.txt                    #NetNTLMv1
hashcat -m 5600 hashes.txt wordlist.txt                    #NetNTLMv2
hashcat -m 13100 hashes.txt wordlist.txt                   #Kerberos 5 TGS-REP etype 23
hashcat -m 7500 hashes.txt wordlist.txt                    #Kerberos 5 AS-REQ Pre-Auth etype 23
hashcat -m 7300 hashes.txt wordlist.txt                    #IPMI2 RAKP HMAC-SHA1
hashcat -m 15300 hashes.txt wordlist.txt                   #DPAPI masterkey file v1
hashcat -m 15900 hashes.txt wordlist.txt                   #DPAPI domain backup key
hashcat -m 2100 hashes.txt wordlist.txt                    #Domain Cached Credentials (DCC2)
hashcat -m 2500 -a 3 handshake.hccapx wordlist.txt         #WPA/WPA2 Handshake (old format)
hashcat -m 22000 -a 3 handshake.22000 wordlist.txt         #WPA/WPA2 PMKID/EAPOL (recommended)
hashcat -m 12500 hashes.txt wordlist.txt                   #Kerberos 5 TGS-REP etype 17/18
hashcat -m 16800 hashes.txt wordlist.txt                   #WPA-PMKID (no EAPOL)
hashcat -m 7100 hashes.txt wordlist.txt                    #macOS v10.8+ (PBKDF2-SHA512)
hashcat -m 11600 hashes.txt wordlist.txt                   #7-Zip
hashcat -m 13400 hashes.txt wordlist.txt                   #KeePass 1.x
hashcat -m 13711 hashes.txt wordlist.txt                   #VeraCrypt SHA256 + XTS 512 bit
hashcat -m 11300 hashes.txt wordlist.txt                   #TrueCrypt PBKDF2-SHA512 + XTS
hashcat -m 18300 hashes.txt wordlist.txt                   #BitLocker
hashcat -m 19500 hashes.txt wordlist.txt                   #MS Office 2016
```

## Attack modes availabe are:
```
-a
0 | Straight
1 | Combination
3 | Brute-force
6 | Hybrid Wordlist + Mask
7 | Hybrid Mask + Wordlist
9 | Association
```


