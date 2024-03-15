# PPA
A PPA repository for SecureDNA packages.  Currently built Ubuntu amd64, and tested in 22.04 and later.

SecureDNA is a free, non-profit screening platform designed to safeguard DNA synthesis everywhere.

- You can find information about the project as a whole, including papers and a live demo, at the [main site](https://securedna.org).
- Source code for the client and servers is available in our [monorepo](https://github.com/SecureDNA/SecureDNA).
- To use the production servers with real databases, you'll need to [obtain certificates](https://securedna.org/start/), but you can compile the entire system below and run test servers with test databases and your own certificates.

# Usage

```bash
curl -sSL https://securedna.github.io/ppa/deb/securedna-keyring.gpg | sudo tee /usr/share/keyrings/securedna-keyring.gpg > /dev/null
echo "deb [signed-by=/usr/share/keyrings/securedna-keyring.gpg] https://securedna.github.io/ppa/deb ./" | sudo tee /etc/apt/sources.list.d/securedna.list > /dev/null
sudo apt update
sudo apt install synthclient
```
