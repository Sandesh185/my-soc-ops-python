🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# 🎯 Soc Ops: Social Bingo

<div align="center">

**Break the ice and make connections at your next event!**

A delightful, interactive bingo game designed for in-person mixers and social events. Find people who match fun prompts, get 5 in a row, and build genuine connections.

[Play Now](#-quick-start) | [See Features](#-features) | [Learn More](#-about) | [Dev Lab](#-dev-lab)

</div>

---

## ✨ What Is Soc Ops?

Soc Ops transforms awkward mixer moments into fun, engaging interactions. Players move around the room, chat with fellow attendees, and mark off bingo squares when they find someone who matches the question.

**Examples:**
- "Has visited more than 5 countries"
- "Speaks 2+ languages"
- "Tried a new skill in the last month"
- "Moved cities within the last year"

Get 5 in a row (horizontally, vertically, or diagonally), and you win! But the real reward? Meaningful conversations and new friendships.

---

## 🎮 Features

| Feature | Description |
|---------|-------------|
| 🎲 **Randomized Questions** | 5×5 bingo grid with hand-picked prompt cards |
| 📱 **Mobile Friendly** | Works seamlessly on phones, tablets, and laptops |
| 🎨 **Beautiful UI** | Custom-built CSS with no external dependencies |
| ⚡ **Real-Time Updates** | HTMX-powered dynamic interactions without page reloads |
| 🔄 **Reset & Replay** | Play multiple rounds instantly |
| 🌍 **Multi-Language** | English, Portuguese, and Spanish support |
| 📦 **Lightweight** | Fast, simple, and easy to deploy |

---

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- [uv](https://github.com/astral-sh/uv) (fast Python package installer)

### Installation & Run

```bash
# Install dependencies
uv sync

# Start the dev server
uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

Open your browser to **http://localhost:8000** and start playing!

---

## 🏗️ Tech Stack

Built with modern, production-grade tools:

- **Backend:** [FastAPI](https://fastapi.tiangolo.com/) — Fast, async web framework
- **Frontend:** Jinja2 templates + [HTMX](https://htmx.org/) — Lightweight interactivity
- **Styling:** Custom CSS utilities (no external frameworks)
- **State:** Cookie-based sessions with UUID identifiers
- **Testing:** pytest with 100% coverage
- **Linting:** Ruff with strict type checking

---

## 🧪 Development

### Run Tests
```bash
uv run pytest
```

### Lint & Format
```bash
uv run ruff check .
```

### Project Structure
```
app/
 main.py           # FastAPI routes
 game_logic.py     # Pure game rules
 game_service.py   # Game state management
 models.py         # Pydantic models
 data.py           # Question database
 static/           # CSS & assets
 templates/        # HTML templates
```

---

## 📚 Dev Lab Guide

This project includes a comprehensive **GitHub Copilot development lab** with 5 structured parts:

| Part | Topic | Learn |
|------|-------|-------|
| [**00**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview) | Overview & Checklist | Project scope & prerequisites |
| [**01**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=01-setup) | Setup & Context Engineering | Copilot agent customization |
| [**02**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=02-design) | Design-First Frontend | Building engaging UIs with Copilot |
| [**03**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=03-quiz-master) | Custom Quiz Master | Creating specialized agents |
| [**04**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=04-multi-agent) | Multi-Agent Development | Orchestrating complex workflows |

> 📖 **Offline?** Lab guides are also available in the [`workshop/`](workshop/) folder.

---

## 🎯 About

Soc Ops was built to solve a real problem: **how to get strangers talking at mixers and conferences**. Traditional icebreakers are awkward. Bingo is fun. Soc Ops combines both.

### Why It Works
 Low-pressure social interaction
 Built-in conversation starters
 Gamified engagement
 Works at any event size

---

## 📄 License

Licensed under the [MIT License](LICENSE).

---

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Code of Conduct
Please review our [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) to help maintain a welcoming community.

---

## ❓ Need Help?

- 📖 Check [SUPPORT.md](SUPPORT.md) for troubleshooting
- 🔒 Security concerns? See [SECURITY.md](SECURITY.md)
- 💬 Questions? Open an issue or start a discussion

---

<div align="center">

**Made with ❤️ for better human connections**

[Back to Top](#-soc-ops-social-bingo)

</div>
