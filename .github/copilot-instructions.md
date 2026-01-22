<!-- .github/copilot-instructions.md - guidance for AI coding agents -->
# Copilot instructions — CursoGESPRO_2026

Purpose: give immediate, actionable context so an AI coding agent can be productive.

Quick facts
- Primary artifacts: `ejemplo.ipynb` (exercise notebook), `README.md` (project overview), `Prueba.txt`, and `img/` (assets).
- Repo type: single-repository teaching materials (not a multi-service app).

Big picture
- This repository contains course materials and exercises rather than a runnable application. The canonical work product is the Jupyter notebook `ejemplo.ipynb` (open in VS Code or Jupyter).
- Content lives in notebooks and markdown; changes should preserve pedagogical structure and cell ordering.

What agents should do first
- Look for pedagogical tasks inside `ejemplo.ipynb` before creating new files.
- Update `README.md` when you add or change top-level exercises or images in `img/`.

Project-specific conventions
- Language: Spanish phrasing is used in README and notebook cells; prefer Spanish in edits unless asked otherwise.
- Notebook edits: add new solution cells rather than re-ordering existing cells; avoid removing exercise prompts.
- Images: store and reference images under `img/` with relative paths (e.g., `img/logo.jpg`).

Developer workflows (what works here)
- No build/test harness detected — to run or test content, open `ejemplo.ipynb` in Jupyter/VS Code Notebook and run cells interactively.
- For small text or markdown updates, edit `README.md` directly.

Integration and external dependencies
- No explicit dependency files (no `requirements.txt` found). If a notebook requires packages, document them in `README.md` or add a `requirements.txt`.

Examples of common tasks
- Add an exercise: insert a new markdown cell titled "Ejercicio N" in `ejemplo.ipynb`, add related code cells, commit with a Spanish summary.
- Fix a broken image link: place the image in `img/` then update the markdown reference in `README.md` or the notebook.

Edge cases and constraints
- Preserve notebook cell metadata where possible (outputs can be cleared only when explicitly asked).
- Keep PRs focused: one pedagogical change per PR makes reviews easier.

If you need more context
- Inspect `ejemplo.ipynb` for exercise structure and `README.md` for project overview.
- Ask the repository owner whether to add a `requirements.txt` for reproducibility.

If merging existing agent guidance
- Merge existing guidance into this file, preserving any repo-specific steps. No additional agent-doc files were found in this scan.

---
Please review and tell me which areas should be expanded (testing, reproducibility, or notebook standards).
