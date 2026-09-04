# Hi, I'm Devine Nyaenya Ngorwe 👋

📍 Nairobi, Kenya · 📬 [devinenyaenya@gmail.com](mailto:devinenyaenya@gmail.com) · 🔗 [LinkedIn](https://www.linkedin.com/in/devine-n-b16776173)

> I build **secure software** — and the proof that it holds.

A decade of running businesses, keeping books, and supporting customers taught me what real security work is about: **accuracy, compliance, and trust.** I'm a security-focused engineer who thinks like both an attacker and a defender, and ships tests, audit logs, and detection rules alongside every control. Based in Nairobi, Kenya, seeking a role in **security operations, application security, IT support, or incident response.**

---

## 🛡️ What I'm working on

| Project | What it is | Stack | Why it matters |
|---|---|---|---|
| **[android-reset-lab](https://github.com/Nyaenya-Devine/android-reset-lab)** | A simulated enterprise MDM device-reset system that **prevents single-person abuse** — dual-control approval, RBAC default-deny, and a tamper-evident hash-chained audit log. | Python (stdlib) + pytest | Ships the **controls** + **the tests that prove they hold**. **6/6 attacks detected, 28 tests passing.** Mapped to MITRE ATT&CK & NIST 800-53. |
| **[android-device-management-tool](https://github.com/Nyaenya-Devine/android-device-management-tool)** | The Android Enterprise (MDM) admin console that pairs with the lab. | TypeScript / Next.js | Full-stack: a security core with a real UI on top. |
| **[endopima-kenya](https://github.com/Nyaenya-Devine/endopima-kenya)** | Bilingual, community-first **endometriosis early-recognition & care-navigation** prototype for Kenya. | HTML | The human side of tech — health-tech that meets people where they are. |

---

## 🧠 The discipline I bring

- **Attacker + defender mindset** — I red-team my own systems (brute force, replay, privilege escalation, after-hours abuse, unknown-device spoofing), then fix what I find and lock it in with regression tests.
- **Security as code, not slides** — PBKDF2+salt auth, `hmac.compare_digest` (timing-safe), role whitelist, session TTL, IP rate limiting, XSS escaping, and AST checks that *ban* dangerous calls.
- **Shipping the receipts** — CI, a live demo, and metrics: **6/6 detection, false positives 14→9, 0 open critical bugs.**

## ⚡ Try the lab (30 seconds)

```bash
git clone https://github.com/Nyaenya-Devine/android-reset-lab.git
cd android-reset-lab
pip install -r requirements.txt
python seed_lab.py           # creates simulated users
python attacker_sim.py       # fires 6 attacks into a hash-chained log
python threat_detection.py   # 6/6 attacks detected
python reports.py            # dashboard
pytest -q                    # 28 passed
```

▶️ **[Watch the 60-second demo](https://github.com/Nyaenya-Devine/android-reset-lab/releases/download/v2.0/android-reset-lab-demo.mp4)**

---

## 📫 Let's connect

- 🔗 **[LinkedIn](https://www.linkedin.com/in/devine-n-b16776173)** — Devine Nyaenya Ngorwe
- ☕ **[GitHub](https://github.com/Nyaenya-Devine)** — github.com/Nyaenya-Devine
- 📄 **[Resume](https://devine-nyaenya-resume.surge.sh)** — host the `resume-site` folder to activate this link
- 📬 **[Email](mailto:devinenyaenya@gmail.com)** — devinenyaenya@gmail.com
