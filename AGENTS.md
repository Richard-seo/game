# Repository Guidelines

## Project Structure & Module Organization
This repository is a single-page canvas game. All HTML, CSS, and JavaScript live in `index.html`.
- `index.html`: UI markup, inline styles, and the game loop/rendering logic.
- Assets are currently generated in code (no external images or audio directories).

## Build, Test, and Development Commands
No build system is required. Open the game directly in a browser:
- `open index.html` (macOS) or `xdg-open index.html` (Linux) to run locally.
- For iterative changes, reload the browser; no bundler or dev server is used.

## Coding Style & Naming Conventions
- Indentation: 2 spaces (see `index.html`).
- JavaScript: use `camelCase` for variables/functions (`drawNormalZombie`, `resizeCanvas`).
- DOM IDs: `camelCase` (`btnLeft`, `btnRight`); CSS classes: lowercase (`hud`, `stat`).
- Keep additions inline with existing structure: styles in `<style>`, logic in the `<script>` IIFE.

## Testing Guidelines
There are no automated tests or frameworks configured. Validate changes manually:
- Launch the page and verify rendering, input handling, and resizing behavior.
- Check mobile/touch behavior (e.g., on a phone or responsive emulator).

## Commit & Pull Request Guidelines
Git history is minimal and does not show a strict convention. Keep commit messages short and descriptive (imperative verbs are preferred).
For pull requests:
- Describe gameplay/UX changes and mention any tuning values you adjusted.
- Include screenshots or short recordings for UI/visual changes.
- Note any performance considerations (canvas draw cost, animation loops).

## Configuration Notes
The game is self-contained and runs offline. Avoid adding external dependencies unless necessary.
