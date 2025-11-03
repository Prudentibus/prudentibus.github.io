# Prudentibus GitHub Pages - Project Context

> This file is automatically loaded at the start of every Claude Code session.
> Use it to define project-specific rules, conventions, and instructions.

## Project Overview

- **Type:** GitHub Pages personal website
- **Framework:** Static HTML/CSS/JS (no build process)
- **Branch Strategy:** Feature branches starting with `claude/`
- **Hosting:** GitHub Pages at `https://prudentibus.github.io`

## File Structure & Rules

### Main Files
- `index.html` - Landing page
- `calculator.html` - Retro calculator demo
- `.claude/context.md` - This file (project rules)

### Naming Conventions
- HTML pages: lowercase with hyphens (e.g., `my-page.html`)
- Assets: Store in `/assets/` directory when needed
  - `/assets/css/` - Stylesheets
  - `/assets/js/` - JavaScript files
  - `/assets/images/` - Images

## Development Rules

### When Creating New Pages:
1. **Always** include responsive meta viewport tag
2. **Use** consistent color scheme (purple gradient theme from index.html)
3. **Keep** all CSS/JS inline for simple pages (or use `/assets/` for shared code)
4. **Test** that it works as a standalone file (GitHub Pages serves static files)

### Coding Standards:
- **Indentation:** 4 spaces
- **Comments:** Add comments for complex logic
- **Browser Support:** Modern browsers (ES6+ is fine)
- **Accessibility:** Include alt text, semantic HTML, ARIA labels where needed

### Git Workflow:
- **Always** develop on `claude/` branches
- **Commit messages:** Follow conventional commits style
  - feat: New feature
  - fix: Bug fix
  - docs: Documentation
  - style: Formatting changes
  - refactor: Code restructuring
- **Push** to branch when ready for review

## Common Tasks

### Task A: "Create a new page"
1. Create HTML file in root directory
2. Use purple gradient theme from `index.html`
3. Add link to new page from `index.html` if it's a main feature
4. Commit with message: `feat: Add [page name]`

### Task B: "Add interactive feature"
1. Check if it fits on existing page or needs new page
2. Use inline JavaScript unless it's >200 lines (then use `/assets/js/`)
3. Include keyboard accessibility
4. Test Easter eggs are discoverable (add hints)

### Task C: "Update styling"
1. Maintain retro/modern aesthetic consistency
2. Use CSS variables for theme colors when adding new pages
3. Ensure responsive design (mobile-first)

## Easter Egg Policy

When adding Easter eggs:
- **Always** include subtle hints in comments or UI
- **Document** Easter eggs in commit messages (spoilers OK there)
- **Keep** them fun and non-offensive
- **Examples:** Konami codes, number sequences, hidden messages

## Questions to Ask User Before Starting

For ambiguous requests, clarify:
- **New page or modify existing?**
- **Design style:** Match existing theme or try something new?
- **Interactivity level:** Static, simple JS, or complex app?
- **Mobile support:** Must work on mobile? (usually yes)

## Tech Stack Preferences

- ✅ Vanilla JavaScript (no frameworks unless requested)
- ✅ CSS3 animations and effects
- ✅ Google Fonts for typography
- ✅ Self-contained files (avoid external dependencies when possible)
- ❌ No build tools (this is a simple static site)
- ❌ No npm/package.json unless specifically needed

## Useful Commands

- Test locally: `python3 -m http.server 8000` (then visit localhost:8000)
- Check file structure: `ls -la`
- Find HTML files: Use Glob with pattern `**/*.html`

## Notes

- This is a personal project for learning and experimentation
- Creativity is encouraged (see calculator.html for example)
- Performance matters less than fun and aesthetics
- GitHub Pages may take 1-2 minutes to update after push

---

**Last Updated:** 2025-11-03
**Maintained by:** Claude Code sessions
