# Bydysawd Website — Build Status & Working Plan

**Working branch:** `website/foundation-2026-11-26`  
**Working area:** `redesign-preview/`  
**Status:** Foundation review — in progress  
**Live-site rule:** Do not change the root-level live website as part of preview work. The redesign remains separate until the creator approves launch.

## Confirmed brand architecture

- **Vizard Comms** — the creative studio behind the intellectual property.
- **Bydysawd** — the master universe and overarching brand.
- **Bydysawd Cymru** — the first regional world.
- **Bydysawd Brainrot Cymru** — the legacy project identity and origin of the universe.
- **Bydysawd Cymru – The First Collection** — the first commercial collection.
- **Y Nos Hiraf** — the first major flagship storyline.

## Existing preview structure

The repository already contains a substantial static-site preview:

- `index.html` — Bydysawd master landing page.
- `bydysawd-cymru/index.html` — first-world overview.
- `the-first-collection/index.html` — collection landing page.
- `characters/index.html` and 39 individual character pages.
- `y-nos-hiraf/index.html` — story hub.
- `y-nos-hiraf/chapter-1/index.html` and `chapter-2/index.html` — current chapter pages.
- `radio-annwn/index.html` — podcast destination.
- `vizard-comms/index.html` — studio destination.
- `assets/css/design-system.css` — shared visual system and styling.
- `assets/characters/` — character artwork and related assets.

## Visual direction

Retain the established dark, cinematic fantasy atmosphere and neon palette. The design should feel distinctive, premium and readable rather than cluttered. Use the approved Bydysawd / Bydysawd Cymru brand architecture and avoid presenting legacy naming as the current master brand.

## Content and canon rules

1. The Master Character Roster controls approved character identities, card numbers and pronunciations.
2. The Master Origin Canon controls locked foundational origins and continuity.
3. Explicit creator decisions take precedence.
4. Individual approved profiles provide the current expanded character detail.
5. Website copy must not turn rumours, legacy wording or unresolved mysteries into established fact.
6. Approved artwork is to be reused and optimised for the web, not regenerated or redesigned without separate creator approval.
7. Keep the five-chapter Y Nos Hiraf arc and its established ending intact.

## Build and quality checklist

### Foundation and structure
- [x] First navigation pass across the seven main hub/index pages. Corrected seven over-traversing relative links on the Radio Annwn page; the remaining chapter and individual profile-page links still need a full sweep.
- [ ] Confirm every image and asset path resolves.
- [ ] Check consistent navigation, footer and page titles across all pages.
- [ ] Check the Bydysawd → Bydysawd Cymru → First Collection hierarchy is immediately clear.
- [ ] Ensure the legacy project name is framed as the origin/previous identity, not the current master brand.

### Content
- [x] Confirmed that 39 individual character profile pages and a character index are present. Full canon-by-canon page audit remains outstanding.
- [x] Corrected the world and collection page count to six recognised factions. The Unfactioned remains a classification / status outside formal allegiance, not a seventh faction. Full faction wording review remains outstanding.
- [ ] Review Bydysawd Cymru world history and terminology.
- [ ] Check Y Nos Hiraf chapter pages against the approved story canon and latest production handovers.
- [ ] Keep unresolved character and story details out of definitive public copy.

### Experience and technical checks
- [ ] Mobile layout and navigation.
- [ ] Accessibility: semantic headings, contrast, keyboard navigation, descriptive image alt text and skip links.
- [ ] Performance: image dimensions, file sizes, loading behaviour and font usage.
- [ ] SEO: unique titles/descriptions, canonical URLs, Open Graph and social-sharing previews.
- [ ] Browser and device checks.
- [ ] Final broken-link and missing-asset sweep.

### Launch gate
- [ ] Creator review of the complete preview.
- [ ] Confirm deployment target, domain and publishing method.
- [ ] Back up the current live site.
- [ ] Merge/publish only after explicit creator approval.
- [ ] Verify the live domain, redirects, HTTPS and all key pages after launch.

## Work completed on this branch\n\n- Added this build-status and launch checklist.\n- Corrected the world and First Collection page metadata, copy and statistics to state six recognised factions.\n- Fixed the Radio Annwn page's relative navigation paths, which previously traversed too far up the directory and would have led to broken links.\n- Confirmed 39 individual character HTML pages plus the character index are present.\n\n## Immediate next action

Run a systematic link/path and content-completeness audit of `redesign-preview/`. Fix issues on this working branch only, preserving the current live website until the creator approves the final launch.
