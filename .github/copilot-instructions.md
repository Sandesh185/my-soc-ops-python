# Soc Ops - Social Bingo Game

## ✅ Development Checklist (Before Commit)
- `uv run ruff check .` — Lint code
- `uv run pytest` — Run tests  
- `uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000` — Verify dev server

## Code Style & Architecture
- **Python**: Type hints (required), Pydantic models (frozen=True), dataclasses for state
- **Formatting**: Ruff (line-length 88, rules: E, F, I, N, W, ARG, UP, ANN) enforces type hints and detects unused variables
- **Backend**: FastAPI + HTMX + Jinja2 templates
- **Frontend**: Custom CSS utilities in `app/static/css/app.css`; no external frameworks
- **State**: Cookie-based sessions, UUID session IDs
- **Logic**: Pure functions in `game_logic.py`, side effects in `game_service.py`

## Workflow Agents
- `/tdd` — Red-green-refactor cycle
- `/ui-review` — Design feedback
- `/quiz-master` — Custom question sets
- `/pixel-jam` — Creative UI themes (avoid AI slop: distinctive fonts, bold colors, contextual aesthetics)

## Design Guide

### Design Philosophy
Avoid generic "AI slop" aesthetics. Create distinctive, cohesive designs that surprise and delight. Every design choice should feel intentional and contextual to the game's social bingo theme.

### Typography
- Choose **beautiful, distinctive fonts**, not generic defaults (Arial, Inter, Roboto, system fonts)
- Use font families that elevate the aesthetic and match the theme personality
- Examples: Cultural aesthetic-inspired fonts, playful fonts for social games, elegant serif or script fonts
- Ensure readability at all sizes; use `font-semibold`, `font-bold` for hierarchy

### Color & Theme
- **Commit to a cohesive aesthetic** via CSS variables (`--primary`, `--accent`, `--bg`, etc.)
- Use **dominant colors with sharp accents** over timid, evenly-distributed palettes
- Draw inspiration from IDE themes, cultural aesthetics, or the game's social context
- Create depth: layer CSS gradients, geometric patterns, or contextual effects
- Avoid: purple gradients on white, overused color schemes, timid pastels

### Motion & Micro-interactions
- Prioritize **CSS-only animations** for Jinja2 templates (no external JS frameworks)
- Focus on **high-impact moments**: orchestrate page load with staggered reveals using `animation-delay`
- One well-executed animated sequence beats scattered, scattered micro-interactions
- Use transitions and transforms for fluid, delightful state changes

### Backgrounds & Atmosphere
- Create **atmosphere and depth** rather than solid colors
- Layer CSS gradients, use geometric patterns, add contextual effects
- Match background treatment to the overall aesthetic and game theme

### Execution
- **Match implementation complexity to vision**: Maximalist designs need elaborate effects; minimalist designs need precision and restraint
- Elegance comes from executing your vision *well*, not from complexity
- Use CSS utilities in `app/static/css/app.css` for consistent, composable styling
- Test designs with actual gameplay; ensure visual beauty doesn't compromise usability

### Anti-patterns to Avoid
- Space Grotesk, Inter, Roboto (generic defaults used repeatedly)
- Purple gradients, flat pastels, evenly-distributed color schemes
- Predictable layouts; cookie-cutter component patterns
- Scattered, unfocused micro-interactions
- Style over substance; beauty that compromises function</content>
<parameter name="filePath">/workspaces/my-soc-ops-python/.github/copilot-instructions.md