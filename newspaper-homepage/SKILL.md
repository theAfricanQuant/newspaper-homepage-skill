---
name: newspaper-homepage
description: Turn a user's reading history, supplied links, or source notes into a polished newspaper-style homepage or digest with verified stories and working source links.
metadata:
  short-description: Generate a newspaper-style homepage
---

# Newspaper Homepage

Create a fresh, readable front page from material the user actually provides or that available tools can access. The visual reference is the morning-newspaper option in [ThariqS/ai-newtab](https://github.com/ThariqS/ai-newtab): a large masthead, a lead story, and a column of briefs. Adapt that editorial structure to the requested medium; do not reproduce the repository's code or assume its browser-extension tools are available.

## Gather and rank material

- Identify what the user wants covered, the relevant time range, location, exclusions, and output format. If they gave browsing history or links, use only the accessible, relevant material. If nothing is available, ask for links or offer a clearly labeled sample based on supplied notes; never imply you inspected private browsing history.
- Read source pages when browsing tools are available. Otherwise work from provided excerpts or notes and label that limitation.
- Rank stories by relevance to the user's demonstrated interests, recency, importance, and diversity. Prefer a few distinct, useful stories over repeated coverage of one topic. Separate news from evergreen recommendations.
- Keep claims traceable. Attach each story's title to a URL that was present in a source you actually read or that the user supplied. Never invent a link, headline attribution, quotation, date, or detail. If sourcing is uncertain, omit the claim or mark it as unverified.
- Summarize in original language. Distinguish reported facts from analysis and keep uncertainty visible.

## Shape the front page

Use the newspaper structure as a starting point, not a rigid template:

1. **Masthead:** publication name, date or edition, and a short descriptive line.
2. **Lead:** the most useful story, with a strong factual headline, concise dek, and source link.
3. **Secondary stories:** a small set of distinct items with clear headlines and one- or two-sentence summaries.
4. **Briefs / reading list:** compact links for other relevant material, each with a reason it matters.
5. **Optional sections:** add topic labels, editor's note, weather, calendar, or a local angle only when requested or supported by available data.

Keep the page scannable. Use a clear hierarchy, concise copy, consistent date formatting, and enough whitespace to distinguish stories. Avoid filler sections when the source material is sparse. Do not manufacture a full newspaper from too few sources.

## Choose the deliverable

- If the user requests a web page or provides an app/repository, follow its existing framework and conventions. Build a responsive front page with semantic headings, accessible contrast, keyboard-visible links, and graceful narrow-screen layout. Keep content data separate from presentation where that fits the project.
- If the user wants a chat digest, render the same editorial hierarchy in Markdown with linked headlines.
- If they request a standalone artifact, save it in the requested location and make the output usable without hidden context.
- For a recurring or history-driven homepage, make the date/edition explicit and keep each item tied to its source. Do not claim automatic updating unless the surrounding system implements it.

## Visual direction

For the reference's specific front-page format, reproduce this hierarchy:

- Put a large, centered editorial strapline above a wide newspaper page. Set its closing phrase in a contrasting coral italic.
- Frame the paper like a browser page with a slim muted toolbar and one tab, then a compact three-part information line.
- Center an oversized serif masthead and short italic motto between fine rules. Follow it with a double-rule edition/date/weather strip.
- Use three desktop columns: a dominant lead story with a drop cap, a narrower secondary-story column with smaller but still bold serif heads and compact briefs, and a slim right rail.
- Put two compact, square-cornered bordered boxes in the right rail, titled **YOUR DAY** and **THE ALMANAC**. Fill them with relevant sourced facts, milestones, or actual calendar items. Never invent appointments, weather, or daily plans to fill these boxes; omit or adapt unsupported rows.
- Use small uppercase red section labels above story heads, near-black serif headlines, warm paper and ink colors, thin column rules, and generous editorial whitespace.

On small screens, preserve the same reading order and stack the columns and rail boxes. Keep contrast accessible and links keyboard-visible. Images are optional; include them only when relevant, accessible, and properly sourced. Avoid fake paper texture, ornamental clutter, tiny low-contrast type, and copied logos or branding.

## Finish

Check every link against the source list and ensure headlines and summaries match what those sources say. Confirm that the page or digest contains no unsupported filler. When implementing in a project, inspect its existing run/build conventions and report what was changed and any verification performed; do not run paid or external publishing actions unless requested.
