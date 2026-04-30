# Linux — Thinking Through Machines

A six-month Linux seminar for students aged 15–18, built around **Kubuntu LTS** and running 4 days per week for 24 weeks. Linux is the vehicle. The destination is epistemic confidence — the ability to face an unknown system, break it, fix it, and walk away knowing more than before.

---

## What is in this repository

| File | Description |
|---|---|
| `index.html` | Course landing page — links to all materials |
| `phase1-teacher-manual.html` | Phase 1: What is this machine? (16 sessions) |
| `phase1-handouts.html` | Phase 1 student handouts — 4 printable sheets |
| `phase2-teacher-manual.html` | Phase 2: Talking to it (24 sessions) |
| `phase2-handouts.html` | Phase 2 student handouts — 5 printable sheets |
| `phase3-teacher-manual.html` | Phase 3: Making it yours (12 sessions) |
| `phase3-handouts.html` | Phase 3 student handouts — 4 printable sheets |
| `phase4-teacher-manual.html` | Phase 4: Build your own machine (8 sessions) |
| `phase4-handouts.html` | Phase 4 student handouts — 4 printable sheets |
| `phase5-teacher-manual.html` | Phase 5: Solving real problems (20 sessions) |
| `phase5-handouts.html` | Phase 5 student handouts — 5 printable sheets |
| `phase6-teacher-manual.html` | Phase 6: The frontier (16 sessions) |
| `phase6-handouts.html` | Phase 6 student handouts — 4 printable sheets |

---

## The six phases

| Phase | Weeks | Sessions | Topics |
|---|---|---|---|
| 1 — What is this machine? | 1–4 | 16 | OS layers, filesystem, users, permissions |
| 2 — Talking to it | 5–10 | 24 | Terminal, file operations, pipes, package manager |
| 3 — Making it yours | 11–13 | 12 | KDE Plasma, dotfiles, PATH, bash scripting |
| 4 — Build your own machine | 14–15 | 8 | Hardware, compatibility, UEFI, assembly, OS install |
| 5 — Solving real problems | 16–20 | 20 | Scripting depth, SSH, networking, processes, logs, git, cron |
| 6 — The frontier | 21–24 | 16 | Local AI, Ollama, final project, demo day |

**Total: 96 sessions across 24 weeks.**

---

## Course format

- **Platform:** Kubuntu LTS
- **Audience:** 15–18 years
- **Schedule:** 4 days per week, 1 hour per session
- **Hardware build:** Weeks 14–15 — students assemble a PC from components (budget €200–350 per build)
- **Final project:** Students build a tool of their own design in Phase 6, presented on demo day

---

## How to use the materials

Each phase has two documents:

**Teacher manual** — full session-by-session guide containing:
- Session overview and preparation notes
- 60-minute timing breakdown (warm-up / concept / exercise / close)
- Full concept delivery text — what to say and draw on the board
- Exercise instructions with expected student questions and answers
- Teacher notes flagging common mistakes, important moments, and what to watch for

**Student handouts** — designed to be printed one set per student per phase:
- Exercise worksheets with answer fields
- Reference cards for the session's key commands
- Vocabulary checklists at the end of each phase
- Reflection questions

All files are standalone HTML — they open in any browser and print cleanly with correct page breaks.

---

## Course philosophy

> "Nothing here is magic. Everything has a reason."

- **Methodical over reactive** — plan before execute, never improvise under pressure
- **Real problems, real tools** — every exercise produces something the student can use
- **No fairytales** — honest assessment of Linux, of AI, of what tools can and cannot do
- **The machine does what you tell it** — that is power, and it comes with responsibility

The course does not teach Linux advocacy. It teaches the habit of approaching an unknown system systematically: read the error, find the root cause, test one change at a time, document what you learn.

---

## Hosting

This repository is designed to be hosted as a static site via **Netlify** (connected to this GitHub repository) or **GitHub Pages**.

To deploy via Netlify:
1. Connect your GitHub account to Netlify
2. Select this repository
3. Set publish directory to `/` (root)
4. Deploy

No build process, no configuration files needed. All files are plain HTML.

---

## License

These materials are shared for educational use. If you use or adapt them, attribution is appreciated.

---

*Built with care. 96 sessions. 24 weeks. One machine assembled from parts, running a local AI model by the end.*
