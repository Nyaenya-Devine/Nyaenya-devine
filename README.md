# Hi, I'm Devine Nyaenya Ngorwe 👋

📍 Nairobi, Kenya · 📬 devinenyaenya@gmail.com · 🔗 [LinkedIn](https://www.linkedin.com/in/devine-n-b16776173)

I build **secure software** — specifically for the messy, high-stakes problem of **who is allowed to do a dangerous thing, and how do we prove it afterwards.**

> **One line:** I'm a security-focused engineer who thinks like both an attacker and a defender, and ships the *proof* — tests, audit logs, and detection rules — alongside the code.

## What I'm working on

| Project | What it is | Stack | Why it matters |
|---|---|---|---|
| **[🛡️ android-reset-lab](https://github.com/Nyaenya-Devine/android-reset-lab)** | A simulated enterprise MDM device-reset system that **prevents single-person abuse** — dual-control approval, RBAC default-deny, tamper-evident hash-chained audit log, and detection of 6 simulated attacks. | Python (stdlib only) + pytest | Ships security *controls* + *the tests that prove they hold*. **6/6 attacks detected, 28 tests passing.** Mapped to MITRE ATT&CK & NIST 800-53. |
| **[📱 android-device-management-tool](https://github.com/Nyaenya-Devine/android-device-management-tool)** | The Android Enterprise (MDM) admin console that pairs with the lab — the human-facing side of device management. | TypeScript / Next.js | Full-stack: a security core with a real UI on top. |
| **[🌍 endopima-kenya](https://github.com/Nyaenya-Devine/endopima-kenya)** | Bilingual, community-first **endometriosis early-recognition & care-navigation** prototype for Kenya. | HTML | A different register — the *human* side of tech. Health-tech that meets people where they are. |

## Why security + operations + health

A decade of running businesses, keeping books, and supporting customers taught me what a lot of security work is really about: **accuracy, compliance, and trust.** Enterprise device reset is a sharpened example of a universal problem — one compromised account shouldn't be a complete weapon. So I build controls (separation of duties, tamper-evident logging, brute-force lockout) that stop a single person from doing irreversible damage, and I prove them by attacking my own work.

I care about health-tech, too (see `endopima-kenya`), because I want to secure the systems that touch people's health and data.

## The discipline I bring

- **Attacker + defender mindset** — I red-team my own systems: brute force, replay, privilege escalation, after-hours abuse, unknown-device spoofing. Then I fix what I find and lock it in with regression tests.
- **Security as code, not slides** — PBKDF2+salt authn, `hmac.compare_digest` (timing-safe), role whitelist, session TTL, IP rate limiting, `html.escape` (XSS), AST-level safety checks that *ban* dangerous calls.
- **Shipping the receipts** — CI tests, a live demo, metrics (`6/6 detection`, `14→9 false positives`, `0 open critical bugs`), and mapping to **MITRE ATT&CK** and **NIST 800-53**.

## How to use the lab (30 seconds)

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

Watch the **[demo video](https://github.com/Nyaenya-Devine/android-reset-lab/releases/download/v2.0/android-reset-lab-demo.mp4)** for the 60-second walkthrough.

## Let's connect

I'm actively looking for a role in **security operations, application security, IT support, or incident response** — ready to bring a decade of operations and client-service discipline to a security-focused team.

- 🔗 **[LinkedIn](https://www.linkedin.com/in/devine-n-b16776173)** — Devine Nyaenya Ngorwe
- ☕ **[GitHub](https://github.com/Nyaenya-Devine)** — github.com/Nyaenya-Devine
- 📄 **[Resume](https://devine-nyaenya-resume.surge.sh)** — host the `resume-site` folder to activate this link
- 📬 **[Email](mailto:devinenyaenya@gmail.com)** — devinenyaenya@gmail.com
