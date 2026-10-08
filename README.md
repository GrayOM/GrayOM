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

### 📬 Security review for your open-source project

Maintainers who want a security review of their project are welcome to reach me at **tmdals7205@gmail.com**.

My approach differs from a code scan in a few ways, and I'm happy to walk through any of them:

- **Lab first:** your software runs in a disposable local lab, and I measure what each role (anonymous, low-privilege, admin) can actually reach before reading code to explain it.
- **Every file read, not a sample:** the whole tree is read, so findings are not limited to the "core" files a reviewer would usually pick.
- **Proof, not pattern matches:** each finding comes with a reproduction, a negative control and the exact code path, and I re-test your patch before it ships.
- **Private and coordinated:** nothing is published until you are ready.

### 🙏 Thanks

Thank you to **[ubicloud](https://github.com/ubicloud)**, **[Countly](https://github.com/Countly)** and **[Paid Memberships Pro](https://github.com/strangerstudios)** for supporting this research, and for working through each fix together.
