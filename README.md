## Hi, I'm GrayOM 👋

I do security research on open-source web software. I reproduce each issue in a local lab, report it privately to the vendor, and follow it through until the fix ships.

### 🔐 Published findings

| Project | Finding | Severity | Reference |
|---|---|---|---|
| [frain-dev/convoy](https://github.com/frain-dev/convoy) | Cross-tenant source IDOR leaks plaintext message broker credentials — **CVE-2026-81505** | High | [GHSA-p5vg-v7mj-f6q4](https://github.com/frain-dev/convoy/security/advisories/GHSA-p5vg-v7mj-f6q4) |
| [Swetrix/swetrix](https://github.com/Swetrix/swetrix) | Unauthenticated read SSRF in `/tools/*` action endpoints — **CVE-2026-81506** | High | [GHSA-fcm9-fvcm-3p55](https://github.com/Swetrix/swetrix/security/advisories/GHSA-fcm9-fvcm-3p55) |
| [NangoHQ/nango](https://github.com/NangoHQ/nango) | Unauthenticated SQL injection in the task orchestrator via Postgres `NOTIFY` | High | [GHSA-8m28-9wcj-v8ww](https://github.com/NangoHQ/nango/security/advisories/GHSA-8m28-9wcj-v8ww) |
| [ubicloud/ubicloud](https://github.com/ubicloud/ubicloud) | Cross-project information disclosure in ubid resolution and audit-log links (4 commits) | — | [#6399](https://github.com/ubicloud/ubicloud/pull/6399) · [#6407](https://github.com/ubicloud/ubicloud/pull/6407) |
| [strangerstudios/paid-memberships-pro](https://github.com/strangerstudios/paid-memberships-pro) | Members' uploaded files (e.g. ID documents) stored at guessable URLs, readable without authentication and kept after account deletion — fixed in **3.8.8** (random per-upload folders, deletion with the account, listing protection backfilled into existing folders). PR: *"Reported by @GrayOM. Thank you!"* | — | [3.8.8 release](https://github.com/strangerstudios/paid-memberships-pro/releases/tag/3.8.8) · [#3847](https://github.com/strangerstudios/paid-memberships-pro/pull/3847) |

### ⏳ In coordinated disclosure

**6** more findings have been confirmed by their vendors and are waiting for publication. Details will appear here once each vendor publishes.

### 🛠️ How I work

- Every report includes a local Docker reproduction, a negative control and the vendor's own code path.
- I re-test the vendor's patch before it ships, and I report it when the fix is incomplete.

### 🙏 Thanks

Thank you to **[ubicloud](https://github.com/ubicloud)** for supporting this research and for the generous follow-up on the fix.
