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

- Every report comes with a working reproduction, a negative control and the exact code path.
- I re-test the vendor's patch before it ships, and I report it when the fix is incomplete.

### 📬 Security review for your open-source project

Maintainers who want a security review of their project are welcome to reach me at **tmdals7205@gmail.com**. My process has a few distinctive points, and I'm happy to explain them in detail:

- **Every file, not a sample:** most AI-agent audits read only part of a codebase, typically the files that look most important. My review runs an exhaustive chain that covers every file of the project, so issues outside the "core" are not missed.
- **A 14-stage review chain:** each project goes through a fixed sequence of stages. Each stage hands its results to the next, from running the software and measuring what each kind of user can reach, through full-tree analysis, to the final verified report.
- **Reproduced before reported:** nothing is reported until it has been reproduced and captured on screen. That keeps false positives rare.
- **Private and coordinated:** nothing is published until you are ready.

### 🙏 Thanks

Thank you to **[ubicloud](https://github.com/ubicloud)**, **[Countly](https://github.com/Countly)** and **[Paid Memberships Pro](https://github.com/strangerstudios)** for supporting this research, and for working through each fix together.
