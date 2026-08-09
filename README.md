# CoreLine PBX

CoreLine PBX is a Debian-based phone-system platform built around Asterisk, a local web administration interface, a user control panel, physical-phone provisioning, and CoreLine softphones.

> **Project status:** Beta. CoreLine is not yet recommended as the only telephone or emergency-calling system for a home, business, school, or public facility.

[Website](https://corelines.xyz) · [Install](#installation) · [Documentation](docs/) · [Report a bug](https://github.com/OWNER/REPOSITORY/issues/new?template=bug-report.yml) · [Request a feature](https://github.com/OWNER/REPOSITORY/issues/new?template=feature-request.yml)

## What CoreLine includes

- Extensions and SIP credentials
- Inbound and outbound routes
- SIP trunks
- IVRs, ring groups, queues, paging, parking, recordings, and voicemail
- User Control Panel (UCP)
- Cisco, Yealink, Grandstream, Polycom, Panasonic, and generic SIP provisioning groundwork
- Cisco XML services, directory, push alerts, ringtones, and backgrounds
- Windows and Android softphones
- PBX ID and CoreLine Connect remote-access testing
- System status, debugging, backups, firewall, and Fail2Ban tools
- Dark navy and teal administration interface

## Installation

CoreLine currently targets **Debian 12 Bookworm** on a dedicated machine, virtual machine, or VPS.

```bash
curl -fsSL https://corelines.xyz/install/install.sh | sudo bash
```

Before using the command, review the installation notes and understand that it changes system packages and telephony configuration:

- [Installation guide](docs/installation.md)
- [Upgrade guide](docs/upgrading.md)
- [Security policy](SECURITY.md)

## Downloads

Official Windows and Android builds should be downloaded from the repository's **Releases** page or from [corelines.xyz](https://corelines.xyz). Each release should include a SHA-256 checksum.

Do not download CoreLine installers or softphones from unofficial mirrors.

## Supported phones

CoreLine contains provisioning groundwork for several Cisco, Yealink, Grandstream, Polycom, Panasonic, and generic SIP devices. Firmware differences can affect individual features.

See [Supported phones](docs/supported-phones.md) before reporting a provisioning problem.

## Getting help

- Search existing GitHub Issues first.
- Use the provided bug-report form for reproducible problems.
- Remove passwords, activation codes, public IP addresses, phone numbers, email addresses, and customer information from logs.
- Security vulnerabilities must be reported privately. Do not open a public issue.

See [SUPPORT.md](SUPPORT.md) and [SECURITY.md](SECURITY.md).

## Emergency calling

CoreLine does not itself provide PSTN connectivity, emergency service, a registered emergency address, or legal compliance. Those depend on the selected trunk provider, location configuration, jurisdiction, network, power, and deployment.

Do not assume that dialing `911`, `112`, or another emergency number will work correctly until it has been configured and tested using a non-emergency test procedure approved by the provider.

## Source and licensing

This public repository contains product documentation, release information, issue templates, and approved downloadable binaries. It intentionally does **not** contain the private CoreLine application source code.

CoreLine is proprietary software and is not an open-source project. See [LICENSE.md](LICENSE.md). Public visibility does not grant permission to copy, modify, redistribute, reverse engineer, or create derivative works.

## Project links

- Website: https://corelines.xyz
- Trunking preview: https://corelines.xyz/trunk/
- Security reporting: [SECURITY.md](SECURITY.md)
- Roadmap: [ROADMAP.md](ROADMAP.md)
- Changelog: [CHANGELOG.md](CHANGELOG.md)

Copyright © CoreLine. All rights reserved.
