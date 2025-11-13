<!-- =========================================================================
.github/SECURITY.md

Copyright © 2025 Network Pro Strategies (Network Pro™)
SPDX-License-Identifier: CC-BY-4.0 OR GPL-3.0-or-later
This file is part of Network Pro.
========================================================================== -->

<sup>[SPDX-License-Identifier](https://spdx.dev/learn/handling-license-info/):
`CC-BY-4.0 OR GPL-3.0-or-later`</sup>

# 🔐 Security Policy

**Network Pro Strategies**  
**Effective Date:** November 2, 2025

&nbsp;

Thank you for taking the time to responsibly disclose any security issues you may find in Network Pro Strategies. The safety of our users and data is a top priority.

---

## Automated Scanning and Audits

Network Pro&trade; maintains continuous security coverage across multiple layers:

| Category | Tool / Workflow | Frequency |
|-----------|----------------|------------|
| **SAST** | GitLeaks, CodeQL | On push, PR, nightly |
| **DAST** | Probely | Weekly (Tuesday, 9 AM UTC) |
| **Dependency Audit** | npm audit | Every build (non-blocking) |
| **Dependency Updates** | Dependabot | As needed |
| **Code Quality** | ESLint, Prettier, etc. (local) | Developer pre-commit |

Results from these scans are surfaced in the GitHub Security tab or workflow artifacts.

---

## 📣 Reporting a Vulnerability

If you discover a security issue, please report it privately:

- **Email**: [security@s.neteng.pro](mailto:security@s.neteng.pro)
- **Subject**: `[SECURITY] Vulnerability Report: [Project Name]`
- **PGP Key**: [PGP-KEY.asc](https://raw.githubusercontent.com/netwk-pro/.github/master/PGP-KEY.asc)
- **PGP Fingerprint:**  
  `B7FE 1D4E 6CAB 3E71 4A9F DF6E 48CB 7290 C00D 0DA5`
- **PGP Setup Guide**: [How to encrypt with PGP (GitHub Wiki)](https://github.com/netwk-pro/netwk-pro.github.io/wiki/Getting-Started-with-PGP)

Email to `s.neteng.pro` addresses is secured by Proton Mail’s built-in encryption. For full end-to-end protection, encrypt your message using our [PGP key](https://raw.githubusercontent.com/netwk-pro/.github/master/PGP-KEY.asc) with your preferred email client or a [GPG-compatible tool](https://gnupg.org).

> **Note:** Proton Mail is used for all addresses under the `s.neteng.pro` domain. Other addresses (e.g., `support@netwk.pro`) support OpenPGP encryption using their published keys, available at [/pgp](https://netwk.pro/pgp).

Please include:

- A clear and descriptive summary of the issue
- Steps to reproduce, if applicable
- Potential impact and any suggested fixes

We treat all security reports seriously and confidentially.

---

## 🔧 Supported Versions

The following repositories are covered under this policy:

- [`netwk-pro/netwk-pro.github.io`](https://github.com/netwk-pro/netwk-pro.github.io)
- [`netwk-pro/blog`](https://github.com/netwk-pro/blog)
- [`netwk-pro/docs`](https://github.com/netwk-pro/docs)

| Project       | Current Version | Supported Versions |
|---------------|------------------|---------------------|
| Main site     | 1.25.11           | ✅ 1.25.x and newer |
| Blog          | 1.5.7            | ✅ 1.5.x and newer |
| Docs          | 1.3.8            | ✅ 1.3.x and newer |
| Any 0.x       | N/A              | ❌ Not supported |

Versions earlier than 1.0.0 are out of scope for support unless a critical vulnerability affects downstream users.

---

## ⏱ Response Timeline

We aim to respond to security disclosures within **5 business days**. You'll receive:

1. An acknowledgment of your report
2. Ongoing updates as we investigate and fix the issue
3. Credit for the discovery (if desired)

Fixes will be released as soon as reasonably possible.

<blockquote>
All support provided—whether through email, GitHub, community forums, or other channels—is offered “as-is” and <strong>does not constitute any warranty, express or implied</strong>. Network Pro&trade;, its affiliates, owners, operators, and contributors make no guarantees regarding response time, resolution, or suitability for any particular purpose.
</blockquote>

&nbsp;

Please see the **[Support Disclaimer](https://netwk.pro/legal#support)** on our [Legal, Copyright, and Licensing](https://netwk.pro/legal) page for full details.

---

## 🤝 Disclosure Policy

We request that you:

- Do **not** publicly disclose the vulnerability until we have confirmed and released a fix.
- Work with us in good faith to minimize risk to users and systems.

Coordinated disclosure helps protect the entire community.

---

_Thank you for contributing to the safety and resilience of Network Pro Strategies._
