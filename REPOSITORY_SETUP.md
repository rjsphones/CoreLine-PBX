# Public Repository Setup

## 1. Create the repository

Suggested name: `coreline-pbx`

Suggested description:

> Official documentation, downloads, issue tracking, and release information for CoreLine PBX.

Create it as a public repository without automatically adding a README, license, or `.gitignore`, because this package already contains them.

## 2. Replace placeholders

Before the first commit, edit:

- `.github/ISSUE_TEMPLATE/config.yml`
- `README.md`
- Replace `OWNER/REPOSITORY` with the real GitHub owner and repository.
- Replace `CORELINE_SUBREDDIT` after the official subreddit is created.
- Confirm the support/security contact at `corelines.xyz`.

## 3. Upload this package

Upload the contents of `CoreLine-Public-GitHub`, including hidden `.github` and `.gitignore` files. Do not place the containing folder itself inside the repository unless you want an extra directory level.

## 4. Repository settings

- Enable Issues.
- Enable Discussions if the team can moderate them.
- Enable Private vulnerability reporting.
- Disable Wikis unless someone will maintain them.
- Add repository topics such as `pbx`, `asterisk`, `voip`, `sip`, `debian`, and `coreline`.
- Add the official website URL.
- Protect the default branch from accidental force-pushes.
- Limit write access to trusted CoreLine developers.

## 5. Create labels

- `bug`
- `enhancement`
- `documentation`
- `security`
- `reliability`
- `phone-compatibility`
- `needs-triage`
- `needs-review`
- `windows-softphone`
- `android-softphone`
- `coreline-connect`
- `skip-changelog`

## 6. Publish binaries safely

Use GitHub Releases. Do not commit EXE, APK, ZIP, signing keys, keystores, or private source to the repository.

For each release:

1. Create a version tag.
2. Mark beta builds as pre-releases.
3. Upload the final signed binaries.
4. Publish SHA-256 checksums.
5. Include known issues and rollback instructions.
6. Download the public assets and verify their checksums.

## 7. Keep source private

Use a completely separate private repository for actual CoreLine source. Never change this public repository to private temporarily to upload source; Git history and collaborator access can create unintended copies.
