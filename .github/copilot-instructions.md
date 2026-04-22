# Soc Ops - Social Bingo Game

## ✅ Development Checklist (Before Commit)
- `uv run ruff check .` — Lint code
- `uv run pytest` — Run tests  
- `uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000` — Verify dev server

## Code Style & Architecture
- **Python**: Type hints, Pydantic models (frozen=True), dataclasses for state
- **Formatting**: Ruff (line-length 88, rules: E, F, I, N, W); imports: stdlib → third-party → local
- **Backend**: FastAPI + HTMX + Jinja2 templates
- **Frontend**: Custom CSS utilities in `app/static/css/app.css`; no external frameworks
- **State**: Cookie-based sessions, UUID session IDs
- **Logic**: Pure functions in `game_logic.py`, side effects in `game_service.py`

## Workflow Agents
- `/tdd` — Red-green-refactor cycle
- `/ui-review` — Design feedback
- `/quiz-master` — Custom question sets
- `/pixel-jam` — Creative UI themes (avoid AI slop: distinctive fonts, bold colors, contextual aesthetics)</content>
<parameter name="filePath">/workspaces/my-soc-ops-python/.github/copilot-instructions.md