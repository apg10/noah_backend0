# Continue Project Rules (Noah Food Frontend)

## Working style
- Always work in small, safe iterations (max 3 files per iteration).
- Prefer editing files directly (produce diffs/edits), not only suggestions.
- Do not rename/move folders or files unless explicitly requested.
- Do not touch secrets (.env, keys, tokens).
- After each iteration, provide:
  1) Files changed
  2) Summary of changes
  3) Validation steps (and commands if available)
  4) Risks/notes

## Frontend conventions (HTML + Tailwind CDN)
- Keep visual output identical unless explicitly asked to redesign.
- Avoid inline <style> and inline Tailwind config when possible; centralize to:
  - styles.css
  - tailwind-config.js (CDN style: tailwind.config = {...})
- Keep imports consistent across all pages (same fonts, same Tailwind CDN inclusion order).

## Validation checklist (manual if commands not available)
- Open each page with Live Server:
  - index.html, admin.html, repartidor.html, perfil.html, estado.html
- Check browser console: 0 errors
- Verify core UI areas:
  - header/nav, cards, buttons, tables, modals (if any)

## When asked to "autofix"
- Apply a change -> validate -> if validation fails, fix -> re-validate.
- If you cannot run commands, ask the user to run them and paste output.