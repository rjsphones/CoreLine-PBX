# CoreLine Support

CoreLine is currently beta software maintained by a small development community.

## Before opening an issue

1. Confirm the CoreLine version.
2. Confirm the Debian version.
3. Restart only the affected service when safe.
4. Check the CoreLine and Asterisk logs.
5. Search existing issues.
6. Remove all credentials and personal information.

## Where to ask

- Reproducible software bug: GitHub bug report
- Phone-model compatibility: GitHub phone compatibility report
- Feature idea: GitHub feature request
- General conversation: CoreLine community/Reddit
- Security vulnerability: private security report
- Account, billing, phone number, or trunking matter: private CoreLine support channel

## Useful diagnostic commands

```bash
systemctl status coreline --no-pager -l
asterisk -rx "core show version"
asterisk -rx "pjsip show endpoints"
asterisk -rx "pjsip show contacts"
journalctl -u coreline -n 150 --no-pager
```

Sanitize output before posting it. See [docs/diagnostics.md](docs/diagnostics.md).

## Unsupported requests

- Help bypassing licensing or access controls
- Stolen carrier or SIP credentials
- Toll-fraud assistance
- Harassment, spoofing, or illegal calling
- Unsupported modified CoreLine binaries
- Emergency-calling certification
