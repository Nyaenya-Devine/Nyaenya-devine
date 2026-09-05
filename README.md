![](https://komarev.com/ghpvc/?username=Nyaenya-Devine&label=Profile%20views&color=0e75b6&style=flat)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/devine-n-b16776173)
[![Resume](https://img.shields.io/badge/Resume-View-green?style=flat)](https://devine-nyaenya-resume.netlify.app/)
[![Security Lab](https://img.shields.io/badge/Lab-28%20tests%20%7C%206%2F6%20detection-brightgreen)](https://github.com/Nyaenya-Devine/android-reset-lab)

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
| **[🛡️ android-reset-lab](https://github.com/Nyaenya-Devine/android-reset-lab)** | Enterprise MDM reset that **prevents single-person abuse** — dual-control, RBAC default-deny, hash-chained audit, 6 attacks | Python stdlib + pytest | **28 tests, 6/6 detection, 9 precise alerts** |
| **[🔐 chokepoint](https://github.com/Nyaenya-Devine/Nyaenya-Devine-chokepoint)** | Least-privilege access-control & tamper-evident audit for humans and AI agents (OWASP Agentic AI ASI03) | TypeScript | Frontier OWASP 2026 |
| **[📱 device-management-tool](https://github.com/Nyaenya-Devine/android-device-management-tool)** | Android Enterprise admin console — UI for the security lab | TypeScript / Next.js | Full-stack |
| **[🌍 endopima-kenya](https://github.com/Nyaenya-Devine/endopima-kenya)** | Bilingual endometriosis early-recognition & care-navigation for Kenya | HTML | Health-tech |

### The discipline I bring

- **Attacker + defender:** Red-team my own systems (brute force, replay, privilege escalation, after-hours) → fix → regression tests
- **Security as code:** PBKDF2+salt, `hmac.compare_digest`, role whitelist, session TTL, IP rate limiting, `html.escape`, AST safety checks
- **Shipping receipts:** CI, live demo, metrics (6/6, 14→9 false positives, 0 critical bugs), MITRE ATT&CK + NIST 800-53 mapping

### How to use the lab (30 sec)

```bash
git clone https://github.com/Nyaenya-Devine/android-reset-lab.git
cd android-reset-lab
pip install -r requirements.txt
python seed_lab.py && python attacker_sim.py && python threat_detection.py && pytest -q
