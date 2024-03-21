# PPA
SecureDNA is a free, non-profit screening platform designed to safeguard DNA synthesis everywhere.

This is a PPA repository for the SecureDNA client and related utilities.  Currently built for Ubuntu amd64 and arm64, and tested in 22.04 and later.

- You can find information about the project as a whole, including papers and a live demo, at the [main site](https://securedna.org).
- To use the client with real databases, you'll need to [obtain certificates](https://securedna.org/start/) using utilities in this PPA.
- Source code for the client and utilities, and for the servers it talks to, is available in our [monorepo](https://github.com/SecureDNA/SecureDNA).

# Usage

```bash
curl -sSL https://securedna.github.io/ppa/deb/securedna-keyring.gpg | sudo tee /usr/share/keyrings/securedna-keyring.gpg > /dev/null
echo "deb [signed-by=/usr/share/keyrings/securedna-keyring.gpg] https://securedna.github.io/ppa/deb ./" | sudo tee /etc/apt/sources.list.d/securedna.list > /dev/null
sudo apt update
sudo apt install synthclient
```
