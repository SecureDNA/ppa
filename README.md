# ppa
A PPA repository for SecureDNA packages

# Usage

```bash
sudo curl -SsL -o /etc/apt/trusted.gpg.d/securedna.gpg https://securedna.github.io/ppa/deb/securedna.gpg
sudo curl -SsL -o /etc/apt/sources.list.d/securedna.list https://securedna.github.io/ppa/deb/securedna.list
sudo apt update
sudo apt install synthclient
```
