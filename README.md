![](https://komarev.com/ghpvc/?username=Nyaenya-Devine&label=Profile%20views&color=0e75b6&style=flat)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/devine-n-b16776173)
[![Resume](https://img.shields.io/badge/Resume-View-green?style=flat)](https://devine-nyaenya-resume.netlify.app/)
[![Security Lab](https://img.shields.io/badge/Lab-47%20tests%20%7C%206%2F6%20detection%20%7C%20P2%20hardened-brightgreen)](https://github.com/Nyaenya-Devine/android-reset-lab)

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
| **[🛡️ android-reset-lab](https://github.com/Nyaenya-Devine/android-reset-lab)** | Enterprise MDM reset that **prevents single-person abuse** — dual-control, RBAC default-deny, hash-chained audit + HMAC, SQLite+JSON, CSRF, rate limiting | Python stdlib + pytest | **47 tests (json+sqlite), 6/6 detection, 9 precise alerts + ledger/self-approval demos** |
| **[🔐 chokepoint](https://github.com/Nyaenya-Devine/Nyaenya-Devine-chokepoint)** | Least-privilege access-control & tamper-evident audit for humans and AI agents (OWASP Agentic AI ASI03) | TypeScript | Frontier OWASP 2026 |
| **[📱 device-management-tool](https://github.com/Nyaenya-Devine/android-device-management-tool)** | Android Enterprise admin console — UI for the security lab | TypeScript / Next.js | Full-stack |
| **[🌍 endopima-kenya](https://github.com/Nyaenya-Devine/endopima-kenya)** | Bilingual endometriosis early-recognition & care-navigation for Kenya | HTML | Health-tech |

### The discipline I bring

- **Attacker + defender:** Red-team my own systems (brute force, replay, privilege escalation, after-hours, ledger tampering, self-approval) → fix → regression tests
- **Security as code:** PBKDF2/Argon2id + salt, `hmac.compare_digest`, role whitelist, session TTL + CSRF, IP rate limiting, `html.escape`, AST safety checks, HMAC-signed audit log
- **Shipping receipts:** CI (pytest + CodeQL + pip-audit + TruffleHog), live demos, metrics (6/6, 14→9 false positives, 0 critical bugs), MITRE ATT&CK + NIST 800-53 mapping
- **Honest limitations:** Document tamper-evident vs tamper-proof, in-memory rate limiting, no MFA yet — shows production thinking

### How to use the lab (30 sec)

```bash
git clone https://github.com/Nyaenya-Devine/android-reset-lab.git
cd android-reset-lab
pip install -r requirements.txt
python seed_lab.py && python attacker_sim.py && python threat_detection.py && pytest -q
python demo_ledger_attack.py    # tamper detected at line 2
python demo_self_approval.py    # self-approval blocked
```

🎥 [Demo Video](https://github.com/Nyaenya-Devine/android-reset-lab/releases/download/v2.0/android-reset-lab-demo.mp4) | 📊 [Release v3.0 P2 Hardened](https://github.com/Nyaenya-Devine/android-reset-lab/releases) | 📝 [Article: How I Fixed 15 Bugs](https://github.com/Nyaenya-Devine/android-reset-lab/blob/main/ARTICLE.md)

### P2 Hardening Highlights (Current)

- **Storage:** JSON + SQLite abstraction (WAL, ACID) via `LAB_STORAGE_BACKEND=sqlite`
- **Negative tests:** 19 attack tests (SQLi, XSS, CSRF, rate limit, ledger tamper, self-approval)
- **Auth rate limiting:** 5 req/60s per IP/user + 10 req/60s web console → 429 + `CSRF_BLOCKED` logging
- **CSRF:** hidden token + `validate_csrf_token` + SameSite Strict + HttpOnly
- **Scanning:** CodeQL + Dependabot + pip-audit + TruffleHog
- **Threat model:** Mermaid diagram with 11 attacks mapped to controls/detection/demo scripts
- **Honest docs:** 13 limitations documented, 2 demos proving detection/blocking

### P3 In Progress (Slow, necessary)

- Argon2id option with PBKDF2 fallback (`LAB_HASH_ALGO=argon2`)
- HMAC-signed audit log (tamper-proof, not just evident)
- TOTP MFA simulation (optional)
- Splunk/SIEM log shipping (stdout JSON)

### Let's connect — Open to SOC, AppSec, Detection roles (Nairobi/Remote)

- 🔗 [LinkedIn](https://www.linkedin.com/in/devine-n-b16776173)
- 📄 [Resume Full](https://devine-nyaenya-resume.netlify.app/) · [One-Page](https://devine-nyaenya-resume.netlify.app/one-page.html)
- 📬 devinenyaenya@gmail.com
