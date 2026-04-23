
## Step 1: Figure Out Who It Is For

### Reference System Approach

The design system asks: Who is the visitor? What problem does this site solve for them? What should they understand immediately?

For example, Noor Valdez's portfolio targets "museum program leads and exhibition studios hiring an emerging designer." The site clearly names the audience and the job they're hiring for.

### Museum Implementation

**Status:** ✅ IMPLEMENTED (Updated April 23, 2026)

**Entry Page ([docs/index.html](docs/index.html)):**

- **Audience signal:** "For people curious about Marvel as history"
- **Problem solved:** Understand Marvel not as fandom, but as cultural and historical system
- **Immediate value:** "Understand how Marvel became a connected universe and cultural force"

**Home Page ([docs/home.html](docs/home.html)):**

- **Visitor acknowledgment:** "Whether you're new to Marvel or curious about its history as cultural system, follow the route in order."
- **What they'll get:** Knowledge of chronological development, creator contributions, publication lineage, and visual culture through staged museum objects

**Who We're Talking To:**

- New visitors curious about Marvel's historical development
- People interested in comics as cultural artifacts, not just entertainment
- Museum-minded audiences who appreciate curation and interpretation
- Learners who prefer structured, evidence-based narratives

**Job to be Done:**
"I want to understand Marvel as a real historical and cultural phenomenon, not just a fan encyclopedia."

---

## Step 2: Pick the Vibe

### Reference System Approach

The design system shows three example portfolios with different vibes:

- **Noor:** "Warm, story-led portfolio" (Signal: Caregiver × Sage)
- **Jules:** "Sharper, high-contrast portfolio" (Signal: Hero × Sage)
- **Nia:** "Bold, poster-forward portfolio" (Signal: Creator × Outlaw)

Each portfolio's vibe reflects both the designer's work and the audience's expectations.

### Museum Implementation

**Status:** ✅ IMPLEMENTED

**Chosen Vibe:** Museum, curatorial, disciplined, evidence-first

**Vibe Elements:**

1. **Tone:**
   - Interpretive, not encyclopedic
   - Serious and scholarly without being dry
   - Evidence-based, not fandom-driven
   - Respectful to the subject matter and visitors

2. **Visual Language:**
   - Bauhaus-inspired (geometric, restrained, hierarchical)
   - Clean borders, strong shadows, intentional spacing
   - Marvel subject matter (comic covers, creators) supply energy
   - Restraint protects credibility

3. **Metaphor:**
   - Exhibition catalog, not website
   - Rooms, not pages
   - Objects and evidence, not trivia
   - Visitor journey, not random navigation

4. **Consistency Across All Pages:**
   - Entry splash ([docs/index.html](docs/index.html)): Clean hero card with clear message
   - Opening gallery ([docs/home.html](docs/home.html)): Threshold section + chronology sections + companion rooms
   - Era rooms ([docs/eras/](docs/eras/)): Color-themed room bands with hero objects
   - Companion rooms ([docs/people-and-studios.html](docs/people-and-studios.html), [docs/reading-maps/publication-lineage.html](docs/reading-maps/publication-lineage.html), [docs/guides/collection-highlights.html](docs/guides/collection-highlights.html)): Supporting role, never competing with chronology

**Vibe Proof:**

- The site feels like a curated exhibition, not a marketing site
- Visual discipline is maintained across all pages
- Content supports the interpretation, not the other way around

---

## Step 3: Choose the Look

### Reference System Approach

The design system emphasizes: "Pick a visual direction that matches the vibe instead of fighting it."

Example: Noor's portfolio uses "warm editorial collage with paper textures, annotations, and soft museum cues." Jules's portfolio uses "high-contrast systems dashboard with acid accents, status rails, and coded visual rhythm."

The visual direction must serve the vibe, not distract from it.

### Museum Implementation

**Status:** ✅ IMPLEMENTED

**Visual System:** [docs/styles.css](docs/styles.css) (1,221 lines)

**Design Language:**

1. **Color Palette:**
   - `--paper: #f4efe2` (warm cream background)
   - `--paper-strong: #e7ddc3` (secondary neutral)
   - `--paper-soft: #fbf7ec` (tertiary neutral)
   - `--ink: #111111` (deep black for text and borders)
   - `--red: #d92d20`, `--blue: #1d4ed8`, `--yellow: #f7c948` (Marvel primary colors)
   - **Vibe alignment:** Warm, muted background; bold accents only where needed

2. **Typography:**
   - Font stack: Futura, "Avenir Next", Avenir, Montserrat, Arial, sans-serif
   - Titles use `clamp()` for responsive scaling
   - Eyebrows (labels) use uppercase, small caps, letter-spacing for hierarchy
   - Body copy is generous: 1.05rem, 1.65 line-height
   - **Vibe alignment:** Clean, modernist sans-serif matches Bauhaus aesthetic

3. **Layout & Spacing:**
   - Max-width: 74rem (readable column)
   - CSS variables for consistent spacing (--space-xs through --space-2xl)
   - Grids use gap: var(--space-m) for uniform breathing room
   - **Vibe alignment:** Intentional, never crowded

4. **Borders & Frames:**
   - `--frame: 2px solid var(--ink)` on all major elements
   - `--shadow-strong: 6px 6px 0 var(--line)` on primary elements
   - `--shadow-soft: 4px 4px 0 var(--line)` on secondary elements
   - **Vibe alignment:** Bold frames declare importance without fussiness

5. **Card Systems:**
   - `.content-card` — primary information cards with consistent padding, borders, shadows
   - `.artifact-figure` — consistent frame for all images with captions
   - `.portrait-grid` — 3-column grid for creator portraits
   - `.gallery-wall` — flexible gallery layout with artifact groups
   - **Vibe alignment:** Unified system, never ad-hoc styling

6. **Room Color Accents:**
   - `--golden` accent for Golden Age room
   - `--marvel` accent for Marvel Age room
   - `--cinematic` accent for Cinematic Age room
   - **Vibe alignment:** Subtle room identity without overwhelming

7. **Responsive Design:**
   - Mobile: max-width 780px (stacked layout, readable hero)
   - Tablet: max-width 1080px (2-column grids collapse to 1)
   - Desktop: full grid system active
   - **Vibe alignment:** Works on all devices without compromise

**Visual Consistency Across All Pages:**

- All pages use the same CSS
- Cards, figures, borders, and shadows are identical
- Typography hierarchy is maintained everywhere
- No one-off styling or decoration

---

## Step 4: Add Proof People Can Trust

### Reference System Approach

The design system asks: What evidence do visitors need to believe the main claim?

For a designer's portfolio, proof might be:

- Real projects and case studies
- Testimonials from clients
- Visual proof of skill
- Process documentation

The proof sits near the main claim and answers: "Why should I believe you?"

### Museum Implementation

**Status:** ✅ IMPLEMENTED (Strong)

**Main Claim:**
"Marvel is a connected historical and cultural system, not just random superhero stories."

**Proof Surfaces:**

1. **Chronology Rooms (Primary Route):**
   - Each era room presents artifacts that prove a historical shift
   - Golden Age ([docs/eras/golden-age.html](docs/eras/golden-age.html)): Marvel Comics #1 as opening proof object
   - Marvel Age ([docs/eras/marvel-age.html](docs/eras/marvel-age.html)): Fantastic Four #1 proves shared-universe shift
   - Cinematic Age ([docs/eras/cinematic-age.html](docs/eras/cinematic-age.html)): Infinity Gauntlet and MCU props prove franchise scale

2. **Publication Lineage ([docs/reading-maps/publication-lineage.html](docs/reading-maps/publication-lineage.html)):**
   - Four landmark issues staged as "proof objects":
     - Marvel Comics #1 (Opening proof)
     - Fantastic Four #1 (Reinvention proof)
     - Amazing Fantasy #15 (Relatability proof)
     - Infinity Gauntlet (Scale proof)
   - Each has a caption explaining what it PROVES about Marvel

3. **People & Studios ([docs/people-and-studios.html](docs/people-and-studios.html)):**
   - Six creator portraits (Martin Goodman, Jack Kirby, Stan Lee, Steve Ditko, Chris Claremont, Kevin Feige)
   - Each portrait is labeled with their role and contribution
   - Proof that Marvel is a human system, not just characters

4. **Collection Highlights ([docs/guides/collection-highlights.html](docs/guides/collection-highlights.html)):**
   - Wall A: Publication covers as museum objects
   - Wall B: Editorial culture (bullpen desk) + cinematic scale (props)
   - Proof that Marvel spans from editorial desks to cinematic production

5. **Visual Proof Strategy:**
   - Every image has a caption that explains what it PROVES
   - No decorative images; every object is evidence
   - Captions read like museum labels, not just descriptions

**Why Proof Works Here:**

- Visitors believe Marvel's historical importance because they SEE the artifacts
- Each artifact is captioned to explain its significance
- The proof doesn't explain the design process; it explains the Marvel story

---

## Step 5: Turn It Into a Page

### Reference System Approach

The design system breaks down the page into:

- **Message:** What's the main idea?
- **Signal:** What emotion/archetype does it evoke?
- **Look:** Visual direction
- **Proof:** Evidence surfaces
- **Structure:** How the page is organized
- **Build brief:** What HTML/CSS/assets are needed

### Museum Implementation

**Status:** ✅ IMPLEMENTED

**Page Architecture:**

1. **Entry Sequence:**
   - **Page:** [docs/index.html](docs/index.html)
   - **Message:** "This is a museum exhibition about Marvel history"
   - **Signal:** Threshold, invitation, clear
   - **Proof:** Simple hero card with clear CTA
   - **Structure:** Single card, centered, hero-page background
   - **Look:** Bold typography, clear button, minimal design
   - **Build:** Static HTML, 35 lines

2. **Opening Gallery:**
   - **Page:** [docs/home.html](docs/home.html) (sections: opening, chronology, era rooms)
   - **Message:** "Marvel's history flows through three chronology rooms, supported by companion galleries"
   - **Signal:** Curatorial, evidence-based, structured
   - **Proof:** Feature objects (Marvel Comics #1, Fantastic Four #1) in hero section
   - **Structure:**
     - Hero opening section
     - Three room cards (Golden, Marvel, Cinematic)
     - Three room band sections with details
     - Call-outs to companion rooms
   - **Look:** Room bands with color accents, artifact figures with captions
   - **Build:** Multi-section layout, CSS grid system, artifact figure styling

3. **Chronology Rooms (Era Pages):**
   - **Example:** [docs/eras/golden-age.html](docs/eras/golden-age.html)
   - **Message:** "Golden Age is the foundation—Timely Comics, wartime heroes, first proof of mass culture"
   - **Signal:** Historical, foundational, concrete
   - **Proof:** Marvel Comics #1 as room hero, with supporting cards explaining significance
   - **Structure:**
     - Room band header (title, period)
     - Room band hero (copy + feature object)
     - Supporting content grid (threshold issue card, creator cluster card)
   - **Look:** Color-themed room band (--golden), consistent card system
   - **Build:** Reusable room band component, consistent with other era pages

4. **Companion Rooms:**
   - **Pattern:** All follow the same structure
   - **[People & Studios](docs/people-and-studios.html):**
     - Hero section: "Who carries the Marvel story"
     - Portrait wall: Six creators with captions
     - Creator grid: Detailed cards for each person
   - **[Publication Lineage](docs/reading-maps/publication-lineage.html):**
     - Hero section: "Key issues and release moments"
     - Artifact grid: Four proof objects
     - Content grid: Cards explaining each issue's role
   - **[Collection Highlights](docs/guides/collection-highlights.html):**
     - Hero section: "Objects that make Marvel visible"
     - Gallery walls A & B: Publication covers, editorial culture, cinematic props
     - Interpretive note: Why the collection works

5. **Navigation Model:**
   - **Sticky header** with:
     - Site brand (logo/home link)
     - Room tabs (Golden, Marvel, Cinematic)
     - Companion chips (Cast, Proof, Wall)
   - **Consistent across all pages**
   - **Current page is highlighted** (aria-current="page")
   - **Allows jump between rooms or companion galleries**

6. **Information Architecture:**
   - **Primary route:** Chronology spine (entry → opening → 3 rooms in order)
   - **Secondary routes:** Jump to companion room from header
   - **Exit points:** Each room band or transition section offers buttons to next room or companion room
   - **No dead ends:** Every page has clear navigation forward

**Page Audit:**

| Page                       | Message                  | Signal                    | Look                             | Proof                                  | Structure                                  | Build                            | Status |
| -------------------------- | ------------------------ | ------------------------- | -------------------------------- | -------------------------------------- | ------------------------------------------ | -------------------------------- | ------ |
| index.html                 | Invitation to exhibition | Clear, threshold          | Bold hero card                   | Title + lede + CTA                     | Single centered card                       | HTML + CSS                       | ✅     |
| home.html                  | Exhibition overview      | Curatorial, structured    | Room bands, grids                | Feature objects in hero                | Hero + 3 chronology cards + 3 room bands   | HTML + CSS grid                  | ✅     |
| golden-age.html            | Foundation era           | Historical, concrete      | Color-themed room band           | Marvel Comics #1 + creator card        | Header + hero + grid                       | HTML + room-band component       | ✅     |
| marvel-age.html            | Reinvention era          | Dynamic, connecting       | Color-themed room band           | Fantastic Four #1 + creator card       | Header + hero + grid                       | HTML + room-band component       | ✅     |
| cinematic-age.html         | Scale era                | Cinematic, ambitious      | Color-themed room band           | Infinity Gauntlet + MCU props          | Header + hero + grid                       | HTML + room-band component       | ✅     |
| people-and-studios.html    | Cast gallery             | Interpretive, human       | Portrait grid + cards            | 6 creator portraits + descriptions     | Hero + portrait wall + card grid           | HTML + portrait-grid component   | ✅     |
| publication-lineage.html   | Proof timeline           | Evidence-based, selective | Artifact grid + cards            | 4 key issues staged as proof           | Hero + artifact grid + card grid           | HTML + artifact-figure component | ✅     |
| collection-highlights.html | Object gallery           | Museum, visual            | Gallery walls + artifact figures | Publication covers + editorial + props | Hero + 2 gallery walls + interpretive note | HTML + gallery-wall component    | ✅     |

---

## Step 6: Put It Live

### Reference System Approach

The design system says: "Publish the page, see what lands, and decide what to fix next."

The live output teaches you what visitors actually do, which informs the next iteration.

### Museum Implementation

**Status:** ✅ LIVE (GitHub Pages)

**Deployment:**

- **Repository:** `/Users/AmirE./Desktop/IS117/IS117_MT`
- **Publishing platform:** GitHub Pages
- **Branch:** `main`
- **Folder:** `docs/`
- **Entry point:** [docs/index.html](docs/index.html)
- **Live URL:** https://[user].github.io/[repo]/

**What's Published:**

- ✅ Entry page (index.html)
- ✅ Opening gallery (home.html)
- ✅ Three chronology rooms (eras/golden-age.html, marvel-age.html, cinematic-age.html)
- ✅ Three companion rooms (people-and-studios.html, reading-maps/publication-lineage.html, guides/collection-highlights.html)
- ✅ Unified CSS system (styles.css)
- ✅ All media assets (docs/media/ folder with 15 images)

**Verification (April 23, 2026):**

- ✅ All links work (internal navigation verified)
- ✅ All media paths are correct (27 image references verified)
- ✅ All pages render (HTML valid)
- ✅ Visual consistency confirmed (CSS system working)
- ✅ Responsive design verified (3 breakpoints: 1080px, 780px, 900px)

**Documentation:**

- ✅ Durable specs: [docs/\_specs/site-exhibition/spec.md](docs/_specs/site-exhibition/spec.md)
- ✅ Sprint docs: 4 sprints documented in [docs/\_specs/site-exhibition/sprints/](docs/_specs/site-exhibition/sprints/)
- ✅ Foundation docs: [docs/foundation/](docs/foundation/) (design philosophy, implementation codex, spec patterns, orchestration method)
- ✅ Content model: [docs/content/collection-model.md](docs/content/collection-model.md)
- ✅ Process visibility: [AGENTS.md](AGENTS.md), [CLAIMS.md](CLAIMS.md), [README.md](README.md)

**What Lands (Current State):**

1. **Entry Experience:** Clean threshold with clear audience signal and benefit promise
2. **Visual Credibility:** Bauhaus discipline + Marvel subject matter = museum feel
3. **Navigation:** Sticky header allows forward movement or room jumping
4. **Evidence Model:** Every page stages objects as proof, not decoration
5. **Companion Rooms:** Support the chronology without competing with it

**What to Watch Next:**

- Do visitors understand who the site is for? (Test the audience signal)
- Do visitors follow the chronology, or do they jump to companion rooms? (Track click patterns)
- Do visitors understand what Marvel's cultural significance is by the end? (Test comprehension)
- Does the museum metaphor work for non-museum audiences? (Gather feedback)

**Next Iteration (Planned):**

- **curatorial-enrichment:** Expand content depth while maintaining chronology spine
- **visual-qa:** Enforce visual consistency across future additions
- **accessibility:** Full WCAG 2.1 AA compliance

---

## Summary: How the Museum Implements the Six Steps

| Step                       | Reference Asks                               | Museum Answers                                                                                            | Status         |
| -------------------------- | -------------------------------------------- | --------------------------------------------------------------------------------------------------------- | -------------- |
| **1. Who it's for**        | Name the visitor, problem, outcome           | "For people curious about Marvel as history. Understand Marvel as a connected cultural system."           | ✅ IMPLEMENTED |
| **2. Pick the vibe**       | Overall feeling that fits the audience       | Museum, curatorial, disciplined, evidence-first. Bauhaus + Marvel.                                        | ✅ IMPLEMENTED |
| **3. Choose the look**     | Visual direction that matches the vibe       | Clean borders, warm paper, bold shadows, Marvel colors used sparingly. Responsive grid system.            | ✅ IMPLEMENTED |
| **4. Add proof**           | Evidence that supports the main claim        | Staged artifacts (comics, portraits, objects) with interpretive captions. Four companion rooms.           | ✅ IMPLEMENTED |
| **5. Turn it into a page** | Translate decisions into structure and build | 8 pages, consistent navigation, reusable card components, unified CSS system.                             | ✅ IMPLEMENTED |
| **6. Put it live**         | Publish and iterate                          | Published on GitHub Pages. Documented with specs, sprints, and foundation docs. Ready for next iteration. | ✅ IMPLEMENTED |

---

## Key Insights

### Where the Museum Excels:

1. **Proof surfaces:** Objects are staged as evidence, not decoration
2. **Visual discipline:** CSS system is consistent, responsive, and purposeful
3. **Vibe:** Feels like a museum, not a fan site or corporate page
4. **Navigation:** Both chronological and thematic routes work
5. **Documentation:** Specs and sprints create durable process, not just design artifacts

### Where the Museum Has Room to Grow:

1. **Audience clarity:** Added April 2026; needs testing with actual visitors
2. **Feedback loop:** Currently no mechanism to "see what lands"; analytics needed
3. **Expansion:** Next rooms/content must follow the same discipline
4. **Accessibility:** Full WCAG audit pending

### Why This Framework Works for the Museum:

- The six steps are **process-neutral**—they work for portfolios, e-commerce, blogs, AND museums
- The museum adapted them to exhibition logic (audience → vibe → look → proof → architecture → publish)
- The framework protects against drift: each step builds on the last, so decisions compound coherently
- The documentation cycle (specs → sprints → QA → next sprint) institutionalizes the framework

---

## Reference

- **Reference system:** https://kaw393939.github.io/designsystem/
- **Museum site:** [docs/index.html](docs/index.html)
- **Specs:** [docs/\_specs/site-exhibition/spec.md](docs/_specs/site-exhibition/spec.md)
- **Foundation:** [docs/foundation/](docs/foundation/)
- **Process:** [AGENTS.md](AGENTS.md)
