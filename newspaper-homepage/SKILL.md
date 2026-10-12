---
name: newspaper-homepage
description: Turn supplied links, accessible reading material, or source notes into a verified newspaper-style homepage or digest.
metadata:
  short-description: Generate a newspaper-style homepage
---

# Newspaper Homepage

Create a readable front page from material the user provides or that available tools can access. The visual reference is the morning-newspaper option in [ThariqS/ai-newtab](https://github.com/ThariqS/ai-newtab). Adapt the editorial structure to the requested medium; do not reproduce its code or assume its browser-extension tools are available.

## Gather and rank material

- Identify the subject, relevant time range, location, exclusions, and requested format. Use only accessible, relevant links or material supplied by the user. Never imply you inspected private browsing history.
- Read source pages when browsing tools are available. Otherwise work from supplied excerpts or notes and label that limitation.
- Rank stories by relevance, recency, importance, and diversity. Prefer distinct useful items over repeated coverage.
- Keep claims traceable to sources you actually read or the user supplied. Never invent a link, attribution, quotation, date, or detail. Omit uncertain claims or label them unverified.
- Summarize in original language and keep uncertainty visible.

## Shape the front page

1. **Masthead:** publication name, date or edition, and a short motto.
2. **Lead story:** strong factual headline, concise dek, and source link.
3. **Secondary column:** one smaller headline and concise summary, followed by a few compact briefs.
4. **Right rail:** two compact bordered boxes titled **YOUR DAY** and **THE ALMANAC**.

Keep copy concise, scannable, and source-grounded. Use additional stories only within the secondary column; do not add a second page or a long continuation below the front page.

## Choose the deliverable

- For a web page or app/repository, follow its framework and conventions. Use semantic headings, accessible contrast, keyboard-visible links, and a responsive layout. Keep content separate from presentation where appropriate.
- For a chat digest, use the same hierarchy in Markdown with linked headlines.
- For a standalone artifact, save it in the requested location and make it usable without hidden context.
- For recurring or history-driven content, state the edition date and tie each item to its source. Do not claim automatic updating unless implemented.

## Visual direction

For the reference front page, match this format and scope:

- Begin directly with the newspaper page and its compact three-part information line. Do not add a promotional strapline or fake browser frame or toolbar.
- Center an oversized serif masthead and short italic motto. Follow with the double-rule edition/date strip.
- Use exactly three desktop columns: one dominant lead story with a drop cap; a narrower secondary column with smaller bold serif headlines and compact briefs; and a slim right rail.
- Put only two compact, square-cornered bordered boxes in the rail: **YOUR DAY** and **THE ALMANAC**. Use sourced facts, milestones, or actual calendar items. Never invent appointments, weather, or daily plans; omit unsupported rows.
- Set section labels in small uppercase red type above the story headlines. Keep headlines near-black and serif, on warm paper colors, with thin rules and editorial whitespace.
- Stop after this front page. Do not append feature sections, research lists, biography or teaching panels, source directories, or a footer. Put source links beside the relevant stories or items.
- On narrow screens, stack the same elements in reading order. Keep links keyboard-visible and contrast accessible. Avoid ornamental clutter, tiny low-contrast type, fake paper texture, and copied logos or branding.

## Finish

Check that story claims and links match the source material and that no unsupported filler remains. When implementing in a project, inspect its conventions and report what changed and any verification performed. Do not run paid or external publishing actions unless requested.
