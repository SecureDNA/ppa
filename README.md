# ppa
A PPA repository for SecureDNA packages

# Usage

```bash
sudo curl -SsL https://securedna.github.io/ppa/deb/securedna.gpg | sudo tee /usr/share/keyrings/securedna-keyring.gpg > /dev/null
sudo echo "deb [signed-by=/usr/share/keyrings/securedna-keyring.gpg] https://securedna.github.io/ppa/deb ./" | sudo tee /etc/apt/sources.list.d/securedna.list > /dev/null
sudo apt update
sudo apt install synthclient
```
