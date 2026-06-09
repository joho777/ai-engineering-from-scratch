# 📚 My AI Engineering Learning Log

> A running checklist of everything I should **deeply** understand, lesson by lesson.
> A concept is only checked off after I can (a) restate it in my own words and (b) pass its quiz.

**For every concept, I should be able to explain three things:**
1. **The problem** — why it exists, what breaks without it, the alternatives.
2. **The solution** — how it works, the design decisions, the edge cases.
3. **The broader context** — why it matters, what it impacts downstream.

**My profile:** new to coding & AI · learning style: concept-first, hands-on for the lessons that matter.
**Course size:** 503 lessons across 20 phases (00–19).

**Depth dials I can pull anytime:** `ELI5` · `ELI14` · `ELII (intern)` · `why?` · `deeper` · `next` · `skip` · `where am I?`

---

## Phase 00 · Setup & Tooling  (lesson 1 of 12)

### ✅ Lesson 1 — Dev Environment   `quiz: 5/5` · `restated: ✅`

Concepts mastered:
- [x] **The four-layer stack** — System foundation → Package managers → Runtimes → AI libraries; install bottom-up because each layer depends on the one below. (Package manager *installs* runtime + libraries; runtime *runs* libraries.)
- [x] **Virtual environments** — isolated "desk" per project; solves *version conflicts between projects* (Project A needs NumPy v1, B needs v2).
- [x] **Package managers (`uv`)** — installs runtimes and libraries; "App Store for code."
- [x] **Tensors & GPUs** (preview) — tensor = grid of numbers; GPU does many calcs at once; MPS (Apple) vs CUDA (NVIDIA).
- [x] **Verifying GPU access** — `is_available()` = "can it use the GPU?"; `__version__` = "is it installed?".

What I actually have set up:
- `.venv` course environment (Python 3.12) with NumPy, matplotlib, Jupyter, PyTorch 2.12.
- Apple GPU (MPS) confirmed working.

---

### ✅ Lesson 2 — Git & Collaboration   `quiz: 5/5` · `restated: ✅`

Concepts mastered:
- [x] **Why version control** — a "time machine" for code; snapshots you can return to; enables collaboration & safe experiments.
- [x] **git vs GitHub** — git = the tool on your computer; GitHub = cloud website storing a copy.
- [x] **The four places + commands** — Working Dir → `git add` → Staging → `git commit` → Local Repo → `git push` → Remote.
- [x] **Branches** — `git checkout -b name` creates a parallel universe to experiment safely; `git merge` brings it home.
- [x] **.gitignore** — exclude huge/regenerable files (`.pt`, `.pth`, `.safetensors`, `.venv/`); reason = size + reproducibility, NOT "git can't do binaries."
- [x] **Reading history** — `git log --oneline`; commit = hash + message; `(#NNN)` = a GitHub Pull Request.

Done hands-on: set global git identity (Joseph Hoeksema / joseph.hoeksema@gmail.com).

---

## Up next
- Lesson 3 — GPU Setup & Cloud
- … (9 more in Phase 00)
