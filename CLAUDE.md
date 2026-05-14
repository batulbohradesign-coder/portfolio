# Portfolio

Personal portfolio for bb, UI/UX designer focused on mobile consumer apps.

## Project type

- 7 self-contained HTML files. Each has its own inline CSS and JS.
- NOT a framework project. No React, no build step, no components.

## Folder structure

- index.html (root) — homepage
- case-studies/ — signals.html, figmeet.html, fitness.html
- interactive/ — polaroid.html, speed-scramble.html, breathing-reset.html
- assets/images/ — all images

## Path conventions

- From root: assets/images/file.png and case-studies/file.html
- From case-studies/ or interactive/: ../assets/images/file.png and ../index.html

## Design system

- Fonts: Bricolage Grotesque (headings), Figtree (body), Caveat (handwritten accents)
- Base palette: --bg #FAF8F6, --text #1A1A1A, --text-2 #555, --surface #EEEAE4
- Per-case-study accent colors (intentional, don't unify): signals #C85C3A terracotta, figmeet #00c896 mint, fitness #3D6775 slate teal
- Interactive pages use cream #FAF4E8
- Nav height: 64px across all pages
- Max-width: 1280px (homepage), 920px (case studies)
- Card radii: 24px (tiles), 20px (case study cards), 16px (stat cards)
- Scroll reveal: opacity 0→1, translateY 16px→0, 550ms
- Nav: index.html's nav is canonical. All other pages match exactly — structure, spacing, behavior.
- Mobile (under ~768px): nav collapses into hamburger. Pattern lives in index.html, replicate everywhere.
- Case study layout: 2-column grid (content left, visuals right). All 3 case studies must follow this.

## Voice for case study copy

- First-person, conversational, specific
- Show decisions and tradeoffs, not just outcomes
- No buzzwords ("leveraged," "synergies," "stakeholders")
- Calm, considered, warm

## Don't

- Don't add libraries, frameworks, or build tools
- Don't break HTML files into components
- Don't use lorem ipsum — ask for real copy
- Don't change per-case-study accent colors (terracotta/mint/slate teal are intentional)
- Don't read more file content than needed for a task

## Known UX gaps to fix

- No footer on case study pages — visitors arriving directly can't reach contact or socials
- Page transitions abrupt — index has enter animations, case studies don't
- skincare.html and redesign.html linked on homepage but don't exist yet
- Resume link in footer is # placeholder
- figmeet.html missing favicon
- Case studies missing <meta name="description">
- fitness.html title says "momentum" but filename is fitness.html — pick one

## Working rules

- When fixing one of the UX gaps, fix it across ALL relevant pages in the same session. Don't half-fix.
- When a new pattern is added (e.g. footer), update index.html first as canonical, then propagate.
- Default to terse responses. Skip explanations unless asked.
