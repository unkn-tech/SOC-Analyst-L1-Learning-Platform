# SOC-Analyst-L1-Learning-Platform
# 🛡️ SOC Academy

**A complete learning platform that takes you from zero to job-ready for a SOC Analyst L1 role.**

[![Status](https://img.shields.io/badge/status-active-success)]()
[![Modules](https://img.shields.io/badge/modules-22-cyan)]()
[![Lessons](https://img.shields.io/badge/lessons-100%2B-yellow)]()
[![Quizzes](https://img.shields.io/badge/quizzes-200%2B%20questions-orange)]()
[![License](https://img.shields.io/badge/license-MIT-blue)]()

---

## 🎯 What Is This?

SOC Academy is an interactive web application designed for **complete beginners** — particularly Computer Science undergraduates — who want to build the skills needed for an entry-level Security Operations Center (SOC) role.

It combines structured learning, hands-on labs, simulated SOC investigations, interview preparation, and a truthful resume builder — all in one place.

> **Important:** This platform helps you build foundational and practical skills relevant to SOC Analyst L1 roles. It does not guarantee employment.

---

## 🖼️ Screenshots

| Dashboard | SOC Simulator |
|:---:|:---:|
| ![Dashboard](docs/screenshots/dashboard.png) | ![Simulator](docs/screenshots/simulator.png) |

| Lesson View | Interview Prep |
|:---:|:---:|
| ![Lesson](docs/screenshots/lesson.png) | ![Interview](docs/screenshots/interview.png) |


---

## ✨ Features

### 📚 Structured Learning
- **22 modules** covering everything from cybersecurity basics to job readiness
- **100+ lessons** following a consistent 10-section teaching structure
- **Beginner → Intermediate → Advanced** difficulty progression
- Visual **learning roadmap** with 11 unlockable levels
- Real-world analogies for every concept

### 🧪 Hands-On Practice
- **Interactive SOC Simulator** with realistic alerts to investigate
- **Step-by-step investigations** that teach analyst reasoning
- **Quizzes** with 80% pass threshold and detailed explanations
- **Flashcards** with known/practice tracking
- **Cheat sheets** for networking, Windows events, SIEM queries, and more

### 💼 Career Preparation
- **50+ interview questions** — technical, behavioral, and scenario-based
- **Mock interview system** with keyword-based feedback
- **Truthful resume builder** — never invents metrics or experience
- **Job readiness dashboard** showing skill gaps and next steps
- **Portfolio project guides** with resume bullets

### 📖 Reference Tools
- **Cybersecurity glossary** with simple + technical definitions
- **Global search** across lessons, tools, event IDs, and interview questions
- **Printable cheat sheets** for quick revision

---

## 🚀 Quick Start

This project runs as a **single HTML file** — no build step, no dependencies.

```bash
# Clone the repository
git clone https://github.com/yourusername/soc-academy.git
cd soc-academy

# Open in your browser
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

That's it. The application works immediately with all content seeded and progress saved to `localStorage`.

---

## 🛠️ Tech Stack

### Current Implementation
| Layer | Technology |
|---|---|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| Styling | Custom CSS (dark cybersecurity theme) |
| Data | Seeded JavaScript objects + `localStorage` |
| Deployment | Static file (any web host, GitHub Pages, S3) |

### Planned Production Stack
| Layer | Technology |
|---|---|
| Frontend | React, TypeScript, Tailwind CSS |
| Backend | Python, FastAPI |
| Database | SQLite (dev) → PostgreSQL (prod) |
| Auth | Email/password with JWT |
| Deployment | Docker, Nginx |

---

## 🗺️ Learning Path

```
Level 0   → Cybersecurity Orientation
Level 1   → Networking + Operating Systems
Level 2   → Security Fundamentals
Level 3   → Logs + SIEM
Level 4   → SOC Operations
Level 5   → Alert Triage
Level 6   → Incident Response
Level 7   → Threat Intelligence + MITRE ATT&CK
Level 8   → Advanced SOC Scenarios
Level 9   → Projects
Level 10  → Interview Preparation
Level 11  → Resume + Job Readiness
```

Each level unlocks after completing the previous one.

---

## 📦 Modules

| # | Module | Key Topics |
|---|---|---|
| 0 | Cybersecurity Orientation | CIA Triad, threats, terminology |
| 1 | Networking Fundamentals | TCP/IP, ports, protocols, Wireshark |
| 2 | Operating Systems | Linux CLI, Windows Event Logs |
| 3 | Security Fundamentals | Malware, phishing, attacks |
| 4 | Logs & Log Analysis | Reading and parsing security logs |
| 5 | SIEM Fundamentals | Splunk, Sentinel, Elastic |
| 6 | SOC Operations | Team structure, shift work |
| 7 | Alert Triage | Validation, classification, escalation |
| 8 | Incident Response | NIST/SANS frameworks, playbooks |
| 9 | Threat Intelligence | IOCs, TTPs, enrichment |
| 10 | MITRE ATT&CK | Tactics, techniques, mapping |
| 11 | Endpoint Security | EDR, process trees |
| 12 | Windows Security | Active Directory, Kerberos |
| 13 | Network Security | Firewalls, IDS/IPS |
| 14 | Email Security | Headers, SPF/DKIM/DMARC |
| 15 | Cloud Security | AWS, Azure, IAM |
| 16 | Security Tools | Nmap, Wireshark, CyberChef |
| 17 | Python for SOC | Log parsers, IOC extractors |
| 18 | SOC Projects | Portfolio-ready builds |
| 19 | Interactive SOC Lab | 20+ simulated investigations |
| 20 | Interview Preparation | 50+ questions with model answers |
| 21 | Resume & Job Readiness | Truthful resume builder |

---

## 📂 Project Structure

```
soc-academy/
├── index.html              # Complete application (single file)
├── docs/
│   └── screenshots/        # Demo images for README
├── backend/                # (Planned) FastAPI backend
│   ├── app/
│   │   ├── models/
│   │   ├── routes/
│   │   └── main.py
│   └── requirements.txt
├── frontend/               # (Planned) React frontend
│   ├── src/
│   └── package.json
├── LICENSE
└── README.md
```

---

## 🧪 Sample SOC Investigation

The platform includes a full SOC simulator. Here's a preview of how it works:

```
ALERT #A001 — HIGH SEVERITY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Title:    Multiple failed authentication attempts
Source:   185.220.101.42 (Russia)
Target:   admin@corp.local
Events:   87 failed logins in 10 minutes
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Investigation Steps:
  1. Check for successful logins (Event ID 4624)
  2. Look up source IP reputation (AbuseIPDB, VirusTotal)
  3. Review targeted account privileges
  4. Check for lateral movement
  5. Classify: True Positive / False Positive
  6. Escalate if confirmed compromise
  7. Document findings in ticket
```

Learners click through each step and receive feedback on their reasoning.

---

## 📊 Sample Lesson Structure

Every lesson follows a consistent 10-section format:

1. **Aim** — What you'll learn
2. **Why SOC Analysts Need It** — Relevance to the job
3. **Beginner Explanation** — Plain-language intro
4. **Technical Explanation** — Accurate details
5. **Example** — Realistic scenario
6. **SOC Scenario** — How an analyst encounters it
7. **Hands-on Task** — Practice exercise
8. **Quiz** — 5–10 questions
9. **Interview Questions** — 3–5 common questions
10. **Quick Revision** — 5 bullet points

---

## 🗺️ Roadmap

### ✅ Completed
- [x] Core UI and routing
- [x] Dashboard with progress tracking
- [x] 22-module learning roadmap
- [x] Interactive lesson viewer
- [x] Quiz system with scoring
- [x] SOC alert simulator (8 alerts, 2 full investigations)
- [x] Flashcard system
- [x] Interview prep with 15+ questions
- [x] Mock interview with feedback
- [x] Resume builder (truthful bullets)
- [x] Cheat sheets and glossary
- [x] Global search
- [x] `localStorage` persistence

### 🚧 In Progress
- [ ] Full content for all 100+ lessons
- [ ] 20 complete SOC investigation scenarios
- [ ] 50+ interview questions
- [ ] Python project starter code

### 📋 Planned
- [ ] React + TypeScript frontend migration
- [ ] FastAPI backend with PostgreSQL
- [ ] User authentication (email/password)
- [ ] Admin panel for content management
- [ ] Cloud deployment (Docker + Nginx)
- [ ] Mobile-responsive bottom navigation

---


## 📜 License

**Copyright © 2026 Bhavkirat. All rights reserved.**

This project is proprietary. The source code, design, content, and other materials in this repository may not be copied, modified, distributed, reproduced, or used for commercial purposes without prior written permission from the copyright holder.

Viewing the repository for personal or educational reference is permitted. Any reuse or redistribution of the project's code or substantial content requires prior written permission.


## 🙏 Acknowledgments

- [MITRE ATT&CK](https://attack.mitre.org/) — adversary tactics knowledge base
- [NIST SP 800-61 Rev. 2](https://csrc.nist.gov/publications/detail/sp/800-61/rev-2/final) — Incident Response guide
- [Splunk Documentation](https://docs.splunk.com/Documentation) — SIEM reference
- [VirusTotal](https://www.virustotal.com/) and [AbuseIPDB](https://www.abuseipdb.com/) — threat intelligence
- The open-source cybersecurity community

---

## 👤 Author

- GitHub: https://github.com/unkn-tech

---

## ⚠️ Disclaimer

This platform is an **educational tool**. All security content is designed for:

- ✅ Local lab environments
- ✅ CTF-style practice setups
- ✅ Simulated logs and alerts
- ✅ Intentionally vulnerable applications
- ✅ Authorized practice systems

**Unauthorized access to real systems is illegal and is not endorsed by this project.** Always practice in authorized environments only.

Offensive security techniques are taught **strictly from a defensive perspective** to help analysts understand and detect adversary behavior.

---

## 📬 Support

If this project helped you, consider:
- ⭐ Starring the repository
- 🐛 Reporting bugs
- 📝 Contributing content or fixes
- 📣 Sharing it with others learning cybersecurity

---

<div align="center">

**Built for learners. Designed for defenders.**

[🚀 Get Started](#-quick-start) • [📚 View Modules](#-modules) • [🧪 Try the Simulator](#-sample-soc-investigation)

</div>
