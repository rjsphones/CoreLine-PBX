# Security Policy

## Supported versions

Only the most recent published CoreLine beta is expected to receive security fixes. Older betas may be unsupported.

| Product | Status |
| --- | --- |
| Latest CoreLine PBX beta | Supported for reporting |
| Latest Windows softphone beta | Supported for reporting |
| Latest Android softphone beta | Supported for reporting |
| Older or modified builds | Not supported |

## Report vulnerabilities privately

Do **not** open a public GitHub issue for:

- Authentication bypasses
- Remote command execution
- SIP credential exposure
- Activation-code bypasses
- Portal or PBX account takeover
- Unauthorized calling or toll-fraud paths
- Private data exposure
- Vulnerabilities that could affect deployed PBXs

Use GitHub's private vulnerability-reporting feature when enabled. If it is unavailable, contact the security address published at https://corelines.xyz and use the subject `CoreLine Security Report`.

Include:

- A clear description
- Affected CoreLine product and version
- Reproduction steps
- Expected and actual behavior
- Impact
- Sanitized logs or screenshots
- Whether the issue is already public

Never include real SIP passwords, activation codes, private keys, customer records, or emergency-calling information in a public issue.

## Disclosure expectations

Give CoreLine reasonable time to investigate and prepare a fix before publishing details. CoreLine will try to acknowledge a valid report, reproduce it, assess affected versions, and communicate remediation status.

## Deployment security

Administrators remain responsible for firewall rules, operating-system updates, strong unique credentials, restricted AMI access, backups, trunk limits, monitoring, TLS certificates, and provider security requirements.
