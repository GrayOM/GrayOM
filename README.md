<div align="center">

# Hi, I'm GrayOM 👋

**Vulnerability Assessment** · finding, proving and helping fix real security weaknesses

<br>

[![Published CVEs](https://img.shields.io/badge/Published_CVEs-2-d73a49?style=for-the-badge)](#-published-findings--cves--credits)
[![Credited findings](https://img.shields.io/badge/Credited_findings-5-0969da?style=for-the-badge)](#-published-findings--cves--credits)
[![Bug bounties](https://img.shields.io/badge/Bug_bounties-3-2da44e?style=for-the-badge)](#-bug-bounties)
[![In coordinated disclosure](https://img.shields.io/badge/In_coordinated_disclosure-7-bf8700?style=for-the-badge)](#-in-coordinated-disclosure)

[![Contact](https://img.shields.io/badge/Security_review-tmdals7205%40gmail.com-555555?style=flat-square&logo=gmail&logoColor=white)](mailto:tmdals7205@gmail.com)

</div>

---

I work in **vulnerability assessment**: finding real security weaknesses, proving them, and helping vendors fix them.
My methods and tooling get better every day, and every finding below was confirmed by the vendor.

## 🔐 Published findings — CVEs & credits

| Project | Finding | Severity | Reference |
|---|---|:---:|---|
| [frain-dev/convoy](https://github.com/frain-dev/convoy) | Insecure Direct Object Reference (IDOR) — **CVE-2026-81505** | ![High](https://img.shields.io/badge/-High-d73a49?style=flat-square) | [GHSA-p5vg-v7mj-f6q4](https://github.com/frain-dev/convoy/security/advisories/GHSA-p5vg-v7mj-f6q4) |
| [Swetrix/swetrix](https://github.com/Swetrix/swetrix) | Server-Side Request Forgery (SSRF) — **CVE-2026-81506** | ![High](https://img.shields.io/badge/-High-d73a49?style=flat-square) | [GHSA-fcm9-fvcm-3p55](https://github.com/Swetrix/swetrix/security/advisories/GHSA-fcm9-fvcm-3p55) |
| [NangoHQ/nango](https://github.com/NangoHQ/nango) | SQL Injection | ![High](https://img.shields.io/badge/-High-d73a49?style=flat-square) | [GHSA-8m28-9wcj-v8ww](https://github.com/NangoHQ/nango/security/advisories/GHSA-8m28-9wcj-v8ww) |
| [teableio/teable](https://github.com/teableio/teable) | SQL Injection — base import, physical column name | ![High](https://img.shields.io/badge/-High-d73a49?style=flat-square) | [GHSA-gj7m-w85q-hrj7](https://github.com/teableio/teable/security/advisories/GHSA-gj7m-w85q-hrj7) |
| [teableio/teable](https://github.com/teableio/teable) | Broken Access Control — share-view scope bypass (co-reporter) | ![High](https://img.shields.io/badge/-High-d73a49?style=flat-square) | [GHSA-2333-p777-m9ww](https://github.com/teableio/teable/security/advisories/GHSA-2333-p777-m9ww) |


## 💰 Bug bounties

Findings the vendor rewarded at its own discretion. Amounts are not listed.

| Project | Finding | Severity | Reference |
|---|---|:---:|---|
| [ubicloud/ubicloud](https://github.com/ubicloud/ubicloud) | Information Disclosure (4 commits) | ![Low](https://img.shields.io/badge/-Low-0969da?style=flat-square) | [#6399](https://github.com/ubicloud/ubicloud/pull/6399) · [#6407](https://github.com/ubicloud/ubicloud/pull/6407) |
| [strangerstudios/paid-memberships-pro](https://github.com/strangerstudios/paid-memberships-pro) | Sensitive File Exposure — member file uploads | ![Medium](https://img.shields.io/badge/-Medium-bf8700?style=flat-square) | [3.8.8 release](https://github.com/strangerstudios/paid-memberships-pro/releases/tag/3.8.8) · [#3847](https://github.com/strangerstudios/paid-memberships-pro/pull/3847) |
| [Countly/countly-server](https://github.com/Countly/countly-server) | Details will appear once the advisory is published | — | — |

## ⏳ In coordinated disclosure

> **7** more findings have been confirmed by their vendors and are waiting for publication.
> Details will appear here once each vendor publishes.

## 🛠️ How I work

<table>
<tr>
<td width="50%" valign="top">

**🔍 Every file, not a sample**<br>
Most AI-agent audits read only part of a codebase, typically the files that look most important.
My review runs an exhaustive chain that covers every file of the project, so issues outside the "core" are not missed.

</td>
<td width="50%" valign="top">

**🧩 A 14-stage review chain**<br>
Each project goes through a fixed sequence of stages, and each stage hands its results to the next: from running the
software and measuring what each kind of user can reach, through full-tree analysis, to the final verified report.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**📸 Reproduced before reported**<br>
Nothing is reported until it has been reproduced and captured on screen. That keeps false positives rare,
and every report comes with a working reproduction, a negative control and the exact code path.

</td>
<td width="50%" valign="top">

**🔁 Patch re-testing, private by default**<br>
I re-test the vendor's patch before it ships and report it when the fix is incomplete.
Nothing is published until the vendor is ready.

</td>
</tr>
</table>

## 📬 Security review for your open-source project

Maintainers who want a security review of their project are welcome to reach me at **[tmdals7205@gmail.com](mailto:tmdals7205@gmail.com)**.
My process has a few distinctive points, and I'm happy to explain them in detail.

---

<div align="center">

### 🙏 Thanks

Thank you to **[ubicloud](https://github.com/ubicloud)**, **[Countly](https://github.com/Countly)** and **[Paid Memberships Pro](https://github.com/strangerstudios)**
for supporting this research, and for working through each fix together.

</div>
