# ppa
A PPA repository for SecureDNA packages

# Usage

```bash
curl -sSL https://securedna.github.io/ppa/deb/securedna-keyring.gpg | sudo tee /usr/share/keyrings/securedna-keyring.gpg > /dev/null
echo "deb [signed-by=/usr/share/keyrings/securedna-keyring.gpg] https://securedna.github.io/ppa/deb ./" | sudo tee /etc/apt/sources.list.d/securedna.list > /dev/null
sudo apt update
sudo apt install synthclient
```
