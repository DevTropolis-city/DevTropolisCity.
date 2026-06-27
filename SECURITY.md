# Security Policy

## Supported Versions

DevTropolis is a single static file with no versioned releases yet.
The `main` branch is always the supported version.

| Version | Supported |
| ------- | --------- |
| main    | ✅ |

## Reporting a Vulnerability

DevTropolis runs entirely client-side and only talks to the public,
unauthenticated GitHub REST API — there is no backend, database, or
stored user data. Even so, if you find a security issue (e.g. an XSS
vector via untrusted GitHub profile data, or a dependency risk), please
report it responsibly:

1. **Do not** open a public issue for security vulnerabilities.
2. Open a [private security advisory](../../security/advisories/new) on this repository, or
3. Contact the maintainer directly if advisories are unavailable.

Please include:
- A description of the issue and its impact
- Steps to reproduce
- Any suggested fix, if you have one

We'll do our best to respond promptly and credit reporters in the
[CHANGELOG](CHANGELOG.md) unless you'd prefer to stay anonymous.
