# chezeoff-collab Profile Audit

Date: 2026-06-16

## Public browser state

Observed public profile:

- URL: https://github.com/chezeoff-collab
- Display name: Yaroslav Shobotiuk
- Username: `chezeoff-collab`
- Existing public repository: `fastcup`
- Browser page exposed owner controls such as `Edit profile` and `Customize your pins`, so the browser session appears to be logged in as the target account.

## CLI state

`gh` is currently not authenticated after removing invalid credentials for the
previous suspended accounts. Required before publishing:

```powershell
gh auth login -h github.com -p https -w
gh api user --jq .login
```

The second command must print:

```text
chezeoff-collab
```

## Achievement constraints

Legitimate profile achievements cannot all be forced by one account:

- Starstruck requires real, non-incentivized stars.
- Galaxy Brain requires accepted answers from real discussion authors or maintainers.
- Pair Extraordinaire requires a real consenting coauthor.
- Public Sponsor requires a public paid sponsorship and explicit payment approval.
- Security/Campus/Developer program highlights require program-specific eligibility or manual enrollment.

No fake accounts, automated stars/follows/reactions, unauthorized security tests, or payments should be used.
