# Flowmind

**A quiet, AI-assisted focus companion for the moments your day needs your full attention.**

Built for **Hackhazards '26** — Theme: **01. Human Experience & Productivity**

---

## 🧠 Problem

Most productivity apps pile on features until they become another source of friction: endless settings, notification overload, and to-do lists that never account for how you're actually feeling that day. People don't just need a task list — they need a way to decide *what to do first* when their energy, focus, and time are all limited.

## 💡 Solution

Flowmind is a minimal, single-page focus companion that combines three things people normally juggle across separate apps:

1. **A focus timer** (Pomodoro-style, with adjustable focus/break lengths)
2. **A lightweight task list** for the day
3. **An AI-generated focus plan** — powered by Claude — that looks at your tasks and your current energy level, then suggests a sensible order to tackle them plus one concrete tip to protect your attention.

No sign-up, no clutter — open it and start focusing in seconds.

## ✨ Features

- 🎯 Circular focus timer with three modes (Focus 25 / Focus 15 / Break 5)
- ✎ Simple add/check-off/remove task list
- ◐ Energy/mood check-in (Energized, Steady, Tired, Scattered, Anxious)
- ✦ AI-generated daily plan via the Claude API, personalized to your tasks + energy
- Fully client-side — no backend, no database, no build step

## 🛠️ Tech Stack

- HTML5, CSS3, vanilla JavaScript (no framework — kept intentionally lightweight)
- Anthropic Claude API (`claude-sonnet-4-6`) for the daily plan generation
- Google Fonts (Fraunces, Inter, JetBrains Mono)

## 🚀 Getting Started

This is a single static HTML file — no build step required.

```bash
git clone https://github.com/<your-username>/flowmind.git
cd flowmind
# Open index.html directly in your browser, or serve it locally:
python3 -m http.server 8000
# then visit http://localhost:8000
```

> Note: The "Generate my plan" feature calls the Anthropic API directly from the browser. For local testing/demo purposes this calls `https://api.anthropic.com/v1/messages`; for a production deployment you would proxy this through a small backend to keep API keys secure.

## 🎥 Demo Video

[Link to demo video] — under 5 minutes, public

## 🌐 Live Deployment

[Link to deployed app]

## 🏆 Track / Theme Alignment

- **Theme 01 — Human Experience & Productivity**: Flowmind directly targets habit-building and personal wellbeing by combining focus tooling with an AI assistant tuned to the user's current mental state, rather than treating productivity as a one-size-fits-all checklist.

## 👥 Team

- [Your name] — Solo builder

## 📋 Evaluation Notes

- **Innovation & Originality**: Combines mood-aware planning with a focus timer in one lightweight tool, instead of treating task management and wellbeing as separate concerns.
- **Technical Implementation**: Live Claude API integration for personalized plan generation; fully responsive, zero-dependency front end.
- **Practical Impact**: Usable immediately with zero setup — addresses everyday focus/productivity friction.
- **User Experience & Design**: Calm, distraction-free visual language intentionally designed to avoid the cluttered feel of typical productivity dashboards.

## 📄 License

MIT
