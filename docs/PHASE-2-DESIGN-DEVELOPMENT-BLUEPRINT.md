# Phase 2 — Design and Development Blueprint

**Project:** Bydysawd Brainrot Cymru  
**Repository:** beatsmasterv/bydysawd-brainrot-cymru  
**Working branch:** `redesign/premium-dark-neon`  
**Status:** Phase 1 direction approved; Phase 2 blueprint  
**Production rule:** All redevelopment work stays on this branch. Do not modify `main`, publish to the live GitHub Pages site, or merge without explicit approval.

## 1. Approved creative direction

These decisions are locked and govern all Phase 2 design and build work.

| Area | Approved direction | Practical interpretation |
|---|---|---|
| Visual direction | **Cinematic** | Painterly fantasy atmosphere, dramatic lighting, depth, restrained motion, premium typography and art-led compositions. Retain the recognisable dark-neon identity as an accent language rather than making every surface glow. |
| Navigation | **Hybrid** | Persistent, clear global navigation for core destinations, combined with contextual links, discovery pathways and in-world connections between characters, factions and stories. |
| Character presentation | **Profiles** | Characters are presented as individual profile destinations, not only as a flat trading-card grid. Each profile can connect artwork, identity, lore, faction, abilities, stats and related story content. |

## 2. Product principles

1. **The universe is the product.** The website should feel like an invitation into a coherent Welsh fictional universe, not simply a catalogue of memes.
2. **Discovery before density.** Make the first visit immediately understandable; reveal deeper lore progressively.
3. **Artwork leads.** Use cinematic character and world artwork as the primary visual storytelling device. Interface effects support the art rather than compete with it.
4. **Welsh identity is foundational.** Keep the language, places, folklore and contemporary Welsh references specific and intentional.
5. **Canon over convenience.** Never invent character facts, faction membership, statistics, origins or story connections to fill a layout. Mark missing information for editorial review.
6. **Collectible structure, editorial depth.** Preserve the appeal of rarity, stats and sets while giving each character room to breathe.
7. **Mobile is a first-class experience.** Navigation, reading, artwork and profile interactions must work comfortably on small screens.

## 3. Experience architecture

### Primary navigation

- **Discover** — homepage and current featured entry point.
- **Characters** — searchable/browsable character library.
- **Factions** — faction index and individual faction pages.
- **Stories** — canonical storylines, episodes and mythology.
- **Collections** — sets, seasonal campaigns and collectible groupings.
- **About / The Universe** — concise orientation for new visitors.

The global navigation should remain compact. Contextual navigation should do the deeper work: character profiles link to their faction, stories and collection; faction pages link to members and relevant stories; stories link back to characters and locations.

### Homepage

The homepage should operate as a cinematic front door, with:
- A distinctive hero statement and strong artwork.
- A short, newcomer-friendly explanation of the universe.
- Featured character/profile spotlight.
- Faction discovery.
- Story or campaign spotlight.
- A clear route into the full character library.
- A compact footer with project and social destinations.

Avoid overloading the homepage with every piece of lore. Its job is to establish tone and guide exploration.

### Character library

The library should support:
- Search by character name and known aliases.
- Filters for faction, collection/set and rarity only where verified data exists.
- A responsive profile-led grid with consistent artwork treatment.
- Clear empty states and reset filters.
- A direct route to every individual profile.

Do not display placeholder stats or unverified rarity labels as canon.

### Individual character profile

Recommended content hierarchy:
1. Character artwork, name and identifier.
2. Short hook / epithet.
3. Faction and collection affiliations, where established.
4. Origin and canonical biography.
5. Abilities, strengths, weaknesses and stats, where established.
6. Related characters and story appearances.
7. Previous/next profile navigation and return to library.

Use optional sections: a profile should remain visually complete when some canon fields are not yet available.

### Faction pages

Each page should explain the faction's identity, worldview and place in the wider universe, then surface its confirmed members and relevant stories. Faction names, Welsh spelling, translations and membership must come from the approved canon source.

### Stories and mythology

Create a readable story index and episode/story pages. Support chronology and cross-links to character profiles. Clearly distinguish established Welsh folklore/mythology from original Bydysawd Brainrot Cymru inventions whenever explanatory context is needed.

### Collections and seasonal features

Collections should group characters and stories into a coherent collectible experience. Seasonal campaigns (including Y Nos Hiraf) should be able to have a distinct landing page without fragmenting the core navigation or canonical character records.

## 4. Visual system

### Colour and atmosphere

- Base: deep charcoal/navy backgrounds.
- Surfaces: layered blue-black panels with subtle borders.
- Core identity accents: restrained neon teal, crimson and violet.
- Premium accent: warm antique gold for hierarchy and collectible emphasis.
- Text: high-contrast warm white with muted secondary text.

Use gradients, glows, grain and atmospheric overlays sparingly. Avoid excessive neon outlines, constant animation and generic sci-fi dashboard styling.

### Typography

Use a display face with mythic/editorial character for major headings, a highly legible sans-serif for body copy and a mono face for IDs, labels and collectible metadata. Maintain responsive type scales and comfortable line lengths.

### Artwork

- Prefer approved character artwork and world imagery over emoji or generic stock imagery.
- Use consistent image ratios and deliberate crops in cards and profile headers.
- Keep important character features visible at mobile sizes.
- Provide meaningful alt text; decorative imagery should not create redundant screen-reader noise.
- Do not generate or publish replacement character artwork without checking it against the character bible and approved visual canon.

### Motion and interaction

Use restrained transitions for hover, focus, reveal and navigation. Respect `prefers-reduced-motion`. No essential information should depend on animation or hover.

## 5. Content model and canon integrity

The implementation should be structured so content can be maintained independently of page layout. At minimum, plan for these records:

- **Character:** stable ID, canonical name, aliases, epithet, artwork reference, short description, origin, faction IDs, collection IDs, rarity (if confirmed), stats/abilities (if confirmed), related story IDs, publication status.
- **Faction:** stable ID, canonical Welsh name, approved English rendering (if any), description, artwork, confirmed member IDs, related story IDs.
- **Story:** stable ID, title, sequence/episode, synopsis, canonical text/media references, character IDs, chronology metadata.
- **Collection:** stable ID, title, description, release/season, confirmed member IDs, artwork.

Use stable IDs and explicit relationships rather than matching content by display name. Keep draft/unconfirmed material out of public-facing views.

**Canon source of truth:** the approved Bydysawd Brainrot Cymru character bible, roster and Stories material in the project workspace. The website is a presentation layer, not a new authority for lore. If sources conflict or a field is missing, flag it for review rather than guessing.

## 6. Technical and quality requirements

- Semantic HTML landmarks and a logical heading hierarchy.
- Keyboard-operable navigation, filters and controls with visible focus.
- WCAG 2.2 AA as the accessibility target.
- Responsive layouts tested at narrow mobile, tablet and desktop widths.
- Optimised, appropriately sized images; lazy-load below-the-fold media.
- Avoid unnecessary JavaScript and layout shifts.
- Descriptive page titles, metadata, canonical URLs and social sharing metadata.
- Useful 404/empty states and working internal links.
- No secrets, private workspace links or unpublished personal data in the public repository.

## 7. Delivery sequence

1. **Foundation and design system** — establish shared layout, navigation, typography, colour tokens, buttons, panels and responsive rules.
2. **Homepage** — build the cinematic front door and validate the hybrid navigation model.
3. **Character library** — implement search, verified filters and profile-led browsing.
4. **Character profiles** — build the reusable profile template and connect canonical data.
5. **Faction pages** — create the faction index and reusable faction template.
6. **Stories and mythology** — add the story index, story template and cross-linking.
7. **Collections and seasonal features** — add collection pages and campaign landing-page support.
8. **Quality pass** — mobile, accessibility, performance, metadata, content accuracy and link testing.

## 8. Phase 2 acceptance criteria

Phase 2 is complete when:
- The approved direction is represented in a coherent, documented design system.
- The page architecture and content relationships are defined.
- The first build sequence is clear and technically feasible.
- Existing live content and canon are protected from accidental replacement.
- A development preview can be reviewed independently of the live website.
- No work has been merged into `main` or published to production.

## 9. Current branch baseline

At the start of this blueprint, `redesign/premium-dark-neon` is one commit ahead of `main`, with the existing `redesign-preview.html` added on the development branch. The original `main` branch remains the production baseline. Keep the preview and all subsequent work isolated on the development branch until review and explicit approval.
