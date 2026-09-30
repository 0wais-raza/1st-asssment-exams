<div align="center">

# 🎬 Syllabus — A Cinematic Study Tracker

**A single-file, film-style syllabus tracker. Check off chapters like scenes in a film.**

*HTML · CSS · GSAP 3.13 · Zero build tools · Zero dependencies to install*

</div>

---

## ✨ Features

| | |
|---|---|
| 🎞️ **Fullscreen title card** | Staggered hero text reveal with GSAP timeline |
| 🎛️ **Player deck** | Video-player-style control bar docked at the bottom — progress count, seekbar, exam D-day |
| ⏺️ **Seekbar timeline** | 18 chapter markers; gold = done. Click a marker to jump straight to that chapter |
| ⏱️ **Film-leader intro** | Optional 3-2-1 countdown overlay (skippable — click, Esc, or once per session) |
| 📚 **4 subjects · 18 chapters** | Mathematics (1–4) · Physics (11–14) · Chemistry (2–7) · Computer Science (1–4) |
| ✍️ **Fully editable** | Rename chapters inline, add chapters (+ auto-numbering), delete, per-subject reset |
| 🔍 **Filters** | All / To-do / Done — empty acts dim out |
| 📅 **Exam countdown** | Pick a date → live `D−12` chip, gold at ≤3 days |
| 💾 **Persistence** | Progress saved in `localStorage` — plus JSON export/import backup |
| 🎯 **Accessibility** | `prefers-reduced-motion` support, keyboard-operable checkboxes, ARIA live progress, visible focus |
| 🛡️ **Resilient** | Works with zero JS; if the GSAP CDN fails, everything stays usable (motion is pure enhancement) |

## 🚀 Usage

No install, no build, no server:

```bash
git clone https://github.com/0wais-raza/1st-asssment-exams.git
# then just open index.html in your browser
```

Or double-click `index.html`. That's it.

## 🗂️ Project structure

```
.
├── index.html    # the entire app (HTML + CSS + JS)
├── skills/
│   └── absolute-cinema-ui/
│       └── SKILL.md   # the design skill this UI follows
└── README.md
```

## 🧠 The design skill

This UI was built following a custom **Agent Skill** — [`skills/absolute-cinema-ui/SKILL.md`](skills/absolute-cinema-ui/SKILL.md) — distilled from open skills on GitHub (MengTo's cinematic GSAP systems, `premium-frontend-ui`, `ui-animation`). Its rules:

- Content first — fully visible with zero JavaScript
- Static treatment in CSS, sequenced motion in GSAP
- Effects (vignette, letterbox framing) never reduce text contrast
- Every animation gated behind load checks + `prefers-reduced-motion`

## 🛠️ Tech

- **GSAP 3.13.0** + ScrollTrigger via CDN (free license since 3.13)
- Vanilla **HTML/CSS/JS** — one file, no framework
- **SVG film-leader** countdown (stroke-dashoffset animation)
- Data: `localStorage` with safe parsing + JSON backup files

## 📸 Screenshot

<div align="center">
  <img src="assets/screenshot.png" alt="Cinematic syllabus tracker" width="720">
</div>

## 📄 License

[MIT](LICENSE)

---

<div align="center">
  <sub>Built as a study experiment. Mark your chapters — that's cinema. 🎬</sub>
</div>
