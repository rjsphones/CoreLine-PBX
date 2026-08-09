# CoreLine Release Checklist

## Before packaging

- [ ] Confirm the intended version number everywhere.
- [ ] Run syntax/build checks.
- [ ] Test installation or upgrade on a disposable Debian 12 system.
- [ ] Back up and restore a test PBX.
- [ ] Test administrator and UCP login.
- [ ] Test extension creation and registration.
- [ ] Test inbound, outbound, internal, voicemail, DTMF, paging, parking, and hang-up behavior.
- [ ] Test Windows and Android activation where affected.
- [ ] Test from a different network where remote access is affected.
- [ ] Review logs for exposed passwords or tokens.
- [ ] Confirm no source, secrets, keys, or customer data are packaged.

## Release assets

- [ ] Use exact versioned filenames.
- [ ] Sign binaries using the approved release process.
- [ ] Never upload the signing key or keystore.
- [ ] Generate SHA-256 checksums after the final binary is signed.
- [ ] Prepare release notes, known issues, upgrade instructions, and rollback instructions.
- [ ] Upload binaries as GitHub Release assets, not ordinary repository files.
- [ ] Mark unfinished builds as pre-releases.

## After publishing

- [ ] Download each public asset and verify its checksum.
- [ ] Verify the website download links.
- [ ] Verify installation instructions.
- [ ] Announce the release only after downloads are confirmed.
- [ ] Monitor bug and security reports.
