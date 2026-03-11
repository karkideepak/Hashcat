# Hashcat
password-cracking tool widely used in security testing

## Installation & Setup
### Debian/Ubuntu:
''' javascript
sudo apt update && sudo apt install hashcat
'''
### MacOS:
brew install hashcat

### Using Docker
docker pull hashcat/hashcat
docker run -it --rm hashcat/hashcat --help

### From Source:
git clone https://github.com/hashcat/hashcat.git
cd hashcat
make
./hashcat --help

