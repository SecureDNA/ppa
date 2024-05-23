# PPA
SecureDNA is a free, non-profit screening platform designed to safeguard DNA synthesis everywhere.

This is a PPA repository for the SecureDNA client and related utilities.  Currently built for x86/amd64 (Ubuntu 22.04 and later) and arm64 (Debian Bookworm and later).

It also holds x86/amd64 Red Hat RPMs for CentOS Stream release 9 and later.

## Overview

- You can find information about the project as a whole, including [papers](https://securedna.org/research) and a [live demo](https://securedna.org/demo/), at the [main site](https://securedna.org).
- To use the client with real databases, you'll need to [obtain certificates](https://securedna.org/start/) using utilities in this PPA.
- Docker/podman container images are also available:
  - As a minimal-size image containing just `synthclient`: `docker pull ghcr.io/securedna/synthclient`
  - As an image containing both `synthclient` and the tools required to request a certificate and generate authorization tokens: `docker pull ghcr.io/securedna/synthclient-tools`
- Source for the client and servers is available in our [monorepo](https://github.com/SecureDNA/SecureDNA).

## Ubuntu users:  Adding the PPA to your system and installing its contents

```bash
curl -sSL https://securedna.github.io/ppa/deb/securedna-keyring.gpg | sudo tee /usr/share/keyrings/securedna-keyring.gpg > /dev/null
echo "deb [signed-by=/usr/share/keyrings/securedna-keyring.gpg] https://securedna.github.io/ppa/deb ./" | sudo tee /etc/apt/sources.list.d/securedna.list > /dev/null
sudo apt update
sudo apt install synthclient
```

## Red Hat users:  Adding the public key to your system and installing the RPM

```bash
sudo rpmkeys --import https://securedna.github.io/ppa/rpm/securedna-keyring.asc
sudo yum install -y https://securedna.github.io/ppa/rpm/synthclient-latest.x86_64.rpm
```
