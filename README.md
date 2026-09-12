![](https://komarev.com/ghpvc/?username=Nyaenya-Devine&label=Profile%20views&color=0e75b6&style=flat)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/devine-n-b16776173)
[![Resume](https://img.shields.io/badge/Resume-View-green?style=flat)](https://devine-nyaenya-resume.netlify.app/)
[![Security Lab](https://img.shields.io/badge/Lab-68%20tests%20%7C%20P4%20Cerberus%20%7C%20Merkle%2BCedar-brightgreen)](https://github.com/Nyaenya-Devine/android-reset-lab)

# Hi, I'm Devine Nyaenya Ngorwe 👋

> **Security-focused engineer who thinks like both attacker and defender — and ships the proof (tests, audit logs, detection rules) alongside the code.**

📍 Nairobi, Kenya · 📬 [devinenyaenya@gmail.com](mailto:devinenyaenya@gmail.com) · 🔗 [LinkedIn](https://www.linkedin.com/in/devine-n-b16776173) · 📄 [Resume](https://devine-nyaenya-resume.netlify.app/) · ☕ [GitHub](https://github.com/Nyaenya-Devine)

### Quick Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Nyaenya-Devine&show_icons=true&theme=tokyonight&hide_border=true)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Nyaenya-Devine&layout=compact&theme=tokyonight&hide_border=true)
![Streak](https://github-readme-streak-stats.herokuapp.com/?user=Nyaenya-Devine&theme=tokyonight&hide_border=true)

### What I'm working on

| Project | What it is | Stack | Metrics |
| --- | --- | --- | --- |
| **[🛡️ android-reset-lab](https://github.com/Nyaenya-Devine/android-reset-lab)** · [▶ live console](https://android-reset-lab.vercel.app) | Enterprise MDM reset that **prevents single-person abuse** — P4 Cerberus: Merkle transparency RFC6962, Cedar ABAC 10 policies AuthZEN, risk-adaptive 8 factors, WebAuthn passkeys AAGUID, Play Integrity StrongBox, WYSIWYS tx signing, DPoP RFC9449 | Python + optional argon2-cffi + pytest | **68 tests (P4), 6/6 detection, 0 vulns, 0 medium Bandit** |
| **[🔐 chokepoint](https://github.com/Nyaenya-Devine/chokepoint)** · [▶ live demo](https://chokepoint-demo.vercel.app) | Least-privilege access-control & tamper-evident audit for humans and AI agents (OWASP Agentic AI ASI03) — 5 engines, 5 API routes, 4 dashboards | TypeScript Next 16.3.5 | **0 vulns, lean repo** |
| **[📱 device-management-tool](https://github.com/Nyaenya-Devine/android-device-management-tool)** · [▶ live](https://android-device-management-tool.vercel.app) | Android Enterprise admin console — UI for the security lab | TypeScript / Next.js 16.3.5 | **0 vulns** |
| **[🌍 endopima-kenya](https://github.com/Nyaenya-Devine/endopima-kenya)** | Bilingual endometriosis early-recognition & care-navigation for Kenya | HTML | **CSP self-only, esc() XSS fix** |

### The discipline I bring

- **Attacker + defender:** Red-team my own systems (brute force, replay, privilege escalation, after-hours, ledger tampering, self-approval, HMAC, MFA bypass, clone detection, token binding) → fix → regression tests
- **Security as code:** PBKDF2/Argon2id + salt, `hmac.compare_digest`, role whitelist, session TTL + CSRF, IP rate limiting, `html.escape`, AST safety checks, HMAC-signed audit log, TOTP RFC 6238, Merkle inclusion/consistency proofs, Cedar ABAC fail-closed, WebAuthn counter clone detection, DPoP RFC9449, WYSIWYS tx signing
- **Shipping receipts:** CI (pytest + CodeQL + pip-audit + TruffleHog), live demos (ledger, self-approval, P3, P4 Cerberus), metrics (6/6, 68 tests, 0 vulns), MITRE ATT&CK + NIST 800-53 mapping, formal spec
- **Honest limitations:** Document tamper-evident vs tamper-proof (file-based HMAC vs KMS), in-memory rate limiting vs Redis, plaintext TOTP secret vs encrypted, Argon2 fallback vs required — shows production thinking

### Try the hosted consoles (zero setup)

- **Android Reset Lab** (simulation): <https://android-reset-lab.vercel.app> — sign in with `que` / `LabRat!2026` (also `ops` / `OpsOps!123`, `analyst` / `Analyst!2026`). State resets on cold start by design. Simulation-only, no real device touch.
- **Chokepoint** (demo console): <https://chokepoint-demo.vercel.app> — one-click demo account on the login screen.

### How to use the lab (30 sec, local)

```bash
git clone https://github.com/Nyaenya-Devine/android-reset-lab.git
cd android-reset-lab
pip install -r requirements.txt  # includes argon2-cffi optional
python seed_lab.py && python attacker_sim.py && python threat_detection.py && pytest -q
python demo_ledger_attack.py    # tamper detected at line 2
python demo_self_approval.py    # self-approval blocked
python demo_p3_hardening.py     # Argon2id + HMAC tamper-proof + TOTP MFA + SIEM shipping
python demo_p4_cerberus.py      # Merkle proofs + Cedar ABAC + risk engine + WebAuthn + attestation + tx signing + DPoP
```

🎥 [Demo Video](https://github.com/Nyaenya-Devine/android-reset-lab/releases/download/v2.0/android-reset-lab-demo.mp4) | 📊 [Release v4.0 P4 Cerberus](https://github.com/Nyaenya-Devine/android-reset-lab/releases/tag/v4.0) | 📝 [Article: How I Fixed 15 Bugs → 68 Tests P4](https://github.com/Nyaenya-Devine/android-reset-lab/blob/main/ARTICLE.md)

### P4 Cerberus Highlights (Current)

- **Merkle transparency log:** RFC6962/RFC9162 append-only, inclusion proof O(log N), consistency proof, checkpoint STH signed, anchoring to Sigstore Rekor
- **Policy-as-code:** Cedar ABAC 10 policies (RBAC+ABAC hybrid, device trust, time fences), AuthZEN PDP/PEP API, bundle SHA, safe AST, fail-closed, decision logs
- **Risk-adaptive auth:** 8 factors (IP reputation, geo velocity, device trust score, time anomaly, failure streak, privilege escalation, new device, MFA age) → step-up MFA
- **WebAuthn passkeys sim:** RP ID origin binding, AAGUID allowlist via FIDO MDS sim, counter clone detection, backup eligibility, UV flags
- **Device attestation sim:** Play Integrity MEETS_BASIC/DEVICE/STRONG, hardware-backed StrongBox/TEE vs Software, trust_score, key attestation chain
- **Transaction signing:** WYSIWYS, HMAC-SHA256, nonce, expiry, replay protection
- **DPoP:** RFC9449 proof-of-possession, jti replay cache, htm/htu binding, short-lived tokens
- **Observability:** Prometheus-style metrics, structured logs, trace IDs
- **Tests:** 68 passed, pip-audit 0 vulns, bandit 0 medium 0 high

### Let's connect — Open to SOC, AppSec, Detection roles (Nairobi/Remote)

- 🔗 [LinkedIn](https://www.linkedin.com/in/devine-n-b16776173)
- 📄 [Resume Full](https://devine-nyaenya-resume.netlify.app/) · [One-Page](https://devine-nyaenya-resume.netlify.app/one-page.html)
- 📬 devinenyaenya@gmail.com
