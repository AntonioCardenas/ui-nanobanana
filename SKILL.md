---
name: ui-nanobanana
description: >-
  The ultimate anti-slop UI & frontend art-direction skill powered by high-resolution Google Gemini
  media and reasoning models (Nano Banana 2.1, Nano Banana Pro, Nano Banana 2 Lite, Gemini Omni 1.2 Flash,
  Gemini 4 Carbon, Gemini 4 Argon, Gemini 4 Neon, Gemini 4 Hydrogen). Combines Taste Skill's gallery-proven
  art direction (Subject Inventory, Competitor Test, 2-Line Copy Arithmetic, One Live Thing, Composition
  Variety) with Impeccable's deterministic DESIGN.md / PRODUCT.md guardrails, 18+ design sub-commands
  (/ui audit, /ui normalize, /ui polish, /ui typeset, /ui animate, etc.), 58 anti-slop rules, and an OP
  high-resolution visual pipeline (2K/4K Hero-first Series Lock, panoramic ratios, photographer-brief
  prompts, zero-cut Omni 1.2 video loops, and Carbon/Argon/Neon/Hydrogen SVG/Three.js/Shaders). Use
  whenever building, redesigning, auditing, or polishing websites, landing pages, dashboards, or web apps
  in any stack (Angular, React, Next.js, Astro, Vue, Svelte, HTML/CSS, Tailwind, GSAP, Lenis).
version: 1.1.0
license: MIT
---

# /ui — Taste + Impeccable + Nano Banana (2K/4K OP Edition)

Left to their defaults, coding agents assemble the average of every template they were trained on: a centered three-line headline with an eyebrow badge above it, Inter on a purple-to-blue glow or warm cream-and-terracotta cliché, three identical icon-in-a-square cards, invented metrics, and broken placeholder images.

Even when you strip those tells away with CSS rules alone, a page without real visual substance reads as thin and empty. Studies of 247 curated gallery sites and 91 Awwwards Sites of the Day show that **top-scored pages carry 6–12 cohesive, art-directed visuals**, cover at least half of the first viewport with flagship media on 68% of winners, and pair strict typographic geometry with real motion and interactive proof.

This skill fuses three engines into one deterministic workflow:

1. **Impeccable Deterministic Guardrails (`DESIGN.md` + `PRODUCT.md` + 58 Anti-Slop Rules)** — Locks brand tokens, surface mode (`Persuade`, `Operate`, `Read`, `Experience`), voice, and explicit `anti_references` before a single component or image is created, backed by sub-commands (`/ui audit`, `/ui normalize`, `/ui polish`, `/ui typeset`, `/ui animate`, `/ui bolder`, `/ui quieter`, `/ui overdrive`).
2. **Taste Skill Art Direction & Copy Arithmetic** — Replaces category clichés with a **Subject Inventory** (8–12 facts unique to this client), the **Competitor Test**, **One Live Thing** (a real interactive micro-tool on the page), **Two-Line Headline Arithmetic** ($\le 32$ chars at display size), and **Combinatorial Composition Variety** (no two neighboring sections share a layout; no default left-text/right-image hero reflex).
3. **OP High-Resolution Nano Banana Visual Pipeline** — Turns Google's **Nano Banana 2.1** (`gemini-nano-banana-2.1`), **Nano Banana Pro** (`gemini-3-pro-image`), **Gemini Omni 1.2 Flash** (`gemini-omni-1.2-flash`), and the **Gemini 4 suite** (**Carbon** `gemini-4-carbon`, **Argon** `gemini-4-argon`, **Neon** `gemini-4-neon`, and **Hydrogen** `gemini-4-hydrogen`) into an in-house studio photography, video, and shader department. Instead of stopping at every image or settling for generic stock, it presents **one upfront Batch Media Plan & Cost Quote**, locks the page's palette and lighting into `style.md`, generates the **2K/4K Hero first**, and passes that approved Hero into every subsequent call (**Series Lock**) so all 6–12 visuals share the exact same physical world, color grade, and light direction.

---

## Surface Modes: Page vs. App Screen

Decide the surface mode **first** — it governs layout density, imagery ratio, and motion budget:

| Mode | Surface Kind | Goal | Visual & Imagery Strategy |
|---|---|---|---|
| **Persuade** | Landing page, product launch, marketing site, campaign, pricing | Earn attention, belief, and action | Full art direction: 2K/4K Hero plate ($\ge 40\text{–}60\%$ viewport), 6–10 Series-Locked section visuals, 1 muted video loop, **One Live Thing**, bold composition variety. |
| **Operate** | Dashboard, admin view, analytics, settings, billing, inbox, editor | Complete tasks with speed and clarity | Quiet 1px structural borders, honest tabular data (`tabular-nums`), SVG charts, high scanability. Zero marketing hero bloat; Nano Banana generates crisp avatars, empty-state illustrations, or product object crops only where needed. |
| **Read** | Documentation, technical article, engineering guide, changelog | Comprehension and long-form focus | `65–75ch` measure, crisp typographic hierarchy, Gemini 4 Argon architectural SVGs and Nano Banana 2.1/Pro technical diagrams or editorial header plates. |
| **Experience** | Portfolio, creative studio, lookbook, interactive showcase, event | Immerse the visitor inside the artifact | Artifact leads from `0px` scroll; giant 4K plates, panoramic `21:9` / `4:1` transitions, Omni Flash first-frame-to-video loops, and scroll scenes. |

> **Hybrid rule (SaaS / Product Marketing):** A marketing page that showcases a software product is **Persuade** on the outside, while the product UI fragments inside it follow **Operate** rules. Build product UI fragments in real HTML/CSS + SVG charts (using the app's actual tokens and math that adds up) layered over or beside 2K/4K Nano Banana atmospheric plates — never generate a raster image of fake blurred dashboard text.

---

## The 10-Step Master Run (New Builds & Redesigns)

Follow these steps in order when building or redesigning a surface. Read the linked `references/` files when executing each phase.

### 1. Context, Stack & Subject Inventory
- Check the workspace for `DESIGN.md`, `PRODUCT.md`, and `generations/refs/brand/style.md`. If they exist, load and obey them strictly (see [`references/design-contract.md`](references/design-contract.md)).
- Scan the project's technical stack (`package.json`, `angular.json`, `tailwind.config.*`, CSS variables). Respect the developer's architecture (e.g., Angular v22 zoneless + Signals, React/Next.js, Astro, GSAP, Lenis) — never swap frameworks or add unrequested UI component libraries.
- **Write the Subject Inventory** (see [`references/art-direction-and-copy.md`](references/art-direction-and-copy.md)): list **8 to 12 concrete specifics** that belong to *this* subject and to no competitor (the meaning of its name, its physical materials, its street/origin, real numbers/constraints, rituals, printed artifacts, or exact technical mechanism).

### 2. Write the Argument & Copy Deck (Before Any Markup)
- List the page as **Claims $\rightarrow$ Proof**, one line per section. Delete any section without a distinct claim. Never default to the stock sequence (`Hero -> Logo Bar -> 3 Feature Cards -> Testimonial -> Pricing -> CTA`).
- Apply the **Two-Line Headline Arithmetic** ([`references/art-direction-and-copy.md`](references/art-direction-and-copy.md)):
  $$\text{chars per line} \approx \frac{\text{line width (px)}}{\text{font size (px)} \times k}$$
  Every `h1`–`h6` must fit in **$\le 2$ lines at 1440px, 768px, and 390px**. Keep hero `h1` headlines to **$\le 32$ characters (4–6 words)** with `text-wrap: balance` and an explicit `max-width` in `ch`.
- Place **one supporting sentence** ($\le 22$ words) directly below the `h1` ($32\text{–}48\text{px}$ gap) and **one unmistakable primary action** named for what it does (never `"Get Started"` or `"Learn More"`).
- Never invent social proof (no fake customer logos, fake quotes, `"10,000+ teams"`, or star ratings).

### 3. Lock the Art Direction & Composition Matrix
Select a cohesive combination from [`references/art-direction-and-copy.md`](references/art-direction-and-copy.md) (or honor `DESIGN.md` if pinned):
- **Theme Paradigm:** Pristine Light, Deep Dark (e.g., `#0c1624` base, never pure `#000` + neon glow), Bold Studio Solid, or Quiet Premium Neutral.
- **Hero Scale & Architecture:** Giant Statement, Mid Editorial, or Mini Minimalist. **Do not default to left-text / right-image.** Prefer Centered Over Canvas, Bottom-Left Editorial Over 4K Plate, Asymmetric Split Diptych, Inline Typography Behemoth, or Off-Grid Offset.
- **Section Cadence:** Assign a distinct **Composition Anchor** and **Background Mode** to every section. Neighboring sections must **never** share the same layout family, and at least 3 different anchors must appear across the page.
- If `DESIGN.md` does not exist yet, write it now alongside `generations/refs/brand/style.md` so the design tokens and image generation share one source of truth.

### 4. Find the Idea, Pass the Competitor Test & Design "One Live Thing"
- Complete the **Idea Sentence**:
  > *"On this page, **[specific item from the Subject Inventory]** becomes **[the structural/visual device on the page]**."*
- **The Competitor Test:** Swap a direct competitor's name into that sentence. If it still holds true, your idea is a category cliché — throw it out and pick a sharper item from the inventory.
- **One Live Thing:** Design **one interactive, functional element** built into the page (usually in the Hero or Proof section) that lets the visitor manipulate real domain parameters (e.g., material/finish switcher using Series-Locked Nano Banana plates, interactive signal/latency scrubber, live batch calculator, interactive architectural spec explorer). Must work with a thumb at `390px`, via keyboard (`Tab`/`Enter`/arrows), and render a sensible initial state without waiting for user input.

### 5. Upfront Batch Media Plan & Single Cost-Approval Gate
Pages win or lose on visual substance. Before calling any paid Gemini endpoint, assemble the **Batch Media Plan** (see [`references/nanobanana-visual-pipeline.md`](references/nanobanana-visual-pipeline.md)):
1. Check `generations/refs/` and `generations/refs/sets.json` for real brand logos, product photos, or character references. **Never approximate an existing logo or face in text.**
2. Design the complete visual suite for the surface (typically 4–8 high-res images for a landing page, plus optional video loop and vector/shader code visuals):
   - **Slot 1 (Anchor Hero):** Nano Banana 2.1 (`gemini-nano-banana-2.1`) or Nano Banana Pro (`gemini-3-pro-image`) at `2K` or `4K`, aspect ratio matched to the Hero blueprint (`16:9`, `21:9`, `4:3`, or `3:4`).
   - **Slots 2..N (Section Plates / Crops / Textures / Panoramic Dividers):** Nano Banana 2.1 (`2K`/`4K`, including panoramic `21:9`, `4:1`, `8:1` where appropriate) or Pro (`2K` costs the same 1,120 image tokens as `1K` on Pro — always prefer `2K` over `1K` on Pro!).
   - **Optional Ambient Motion Loop:** Gemini Omni 1.1 Flash (`gemini-omni-1.1-flash`, 5s at `720p` or `1080p`, using Slot 1's generated Hero image as `<FIRST_FRAME>` so the `<video poster>` and first frame match to the pixel).
   - **Optional Code Visuals:** Gemini 4 Argon (`gemini-4-argon`) for intricate SVG schematics, interactive Three.js scenes, or custom GLSL shaders.
3. **Present the Batch Media Plan Table** to the user (listing each slot, model ID, resolution, aspect ratio, brief summary, and itemized + total estimated USD cost) and **wait for one explicit user go-ahead** covering the batch.

### 6. Sequential High-Res Generation with Hero-First Series Lock
Once the user approves the batch:
1. Ensure `generations/refs/brand/style.md` contains the fixed verbatim style block (palette hex codes, lighting direction, camera/lens stock, surface texture, and `anti_references` from `DESIGN.md`). Prepend `style.md` **verbatim** to every image prompt.
2. **Write Photographer's Brief prompts** (Subject + Camera/Focal Length + Lighting Setup + Materiality + Negative-Space Safe Zone for UI text overlay + `"no text, no typography, no watermarks, no UI frames, no hands"`).
3. **Generate Slot 1 (Hero) first.** Save to the target asset folder (e.g., `public/images/` or `generations/`), verify the file is on disk and non-empty, and write its `.json` sidecar with `response_id`.
4. **Lock the Series:** Pass the generated Slot 1 Hero image file in `reference_images` (alongside any brand refs) — or chain via `previous_interaction_id` for state-locked variations — for **Slots 2..N**, running **one generation at a time sequentially**. Every section visual now inherits the Hero's exact lighting, color grade, and physical atmosphere.
5. If the plan includes a **Gemini Omni 1.1 Flash** video loop, pass the approved Hero still as the starting frame (`<FIRST_FRAME>`) so the muted background loop transitions seamlessly from its poster image.

### 7. Build the Interface, Still First
Build the full markup and styles with animations mentally switched off — a page that needs motion to look designed is underbuilt:
- **CSS Custom Properties First:** Define `--bg-ground`, `--bg-surface`, `--bg-elevated`, `--ink-primary`, `--ink-secondary` (tinted from ground hue, never dead grey on color), `--accent-primary`, fluid typography steps (`clamp()`), and spacing tokens from `DESIGN.md`.
- **The Frame Law:** Equal outer margins at `1440px`, `768px`, and `390px`. No section huddled on one side leaving half the viewport accidentally blank — every asymmetry inside the grid is balanced by a visual, list, figure, or second column on the far side. Section vertical rhythm: `120–240px` on desktop.
- **High-Res Image Markup:**
  - Square corners (`border-radius: 0`) by default (94% of Awwwards SOTD winners), or a single consistent radius token across the entire project.
  - Explicit `width` and `height` (or CSS `aspect-ratio`) on every `<img>` and `<video>` to guarantee **0 CLS**.
  - Hero media gets `fetchpriority="high" loading="eager"`; below-the-fold plates get `loading="lazy" decoding="async"`.
  - When placing text over a 2K/4K image, align text inside the engineered negative-space safe zone and add a subtle palette-locked tonal scrim (`linear-gradient` using the ground token's RGB) so contrast is $\ge 4.5:1$ (body) and $\ge 3.0:1$ (display).
- **Theme Browser Surfaces:** Style `::selection`, `:focus-visible`, `caret-color`, custom scrollbars, `text-underline-offset`, and `font-variant-numeric: tabular-nums` using the brand tokens.

### 8. Build the Purposeful Motion Layer
Add motion only after the still layout is complete (see [`references/commands-playbook.md`](references/commands-playbook.md)):
1. **One Signature Authored Move:** A scroll-linked stage, a pinned narrative reveal, a smooth clip-path curtain, or GSAP/Lenis choreography that serves the **Idea Sentence**.
2. **Choreographed Section Entrances:** Stagger heading $\rightarrow$ supporting copy $\rightarrow$ visual (`60–90ms` stagger, `16–24px` rise, exponential ease-out `cubic-bezier(0.16, 1, 0.3, 1)`). Content must never remain `opacity: 0` if JS fails.
3. **Tactile Micro-Feedback:** Crisp hover, active press, and `:focus-visible` states on every control and on **One Live Thing**.
4. **Living Media:** The Omni Flash muted loop (`<video autoplay loop muted playsinline poster="...">`) or a subtle scroll-linked scale/parallax drift (`scale(1.04)`) on the 2K/4K plates.
5. **Accessibility Guardrail:** Respect `@media (prefers-reduced-motion: reduce)` by keeping opacity/color changes and zeroing travel distance.

### 9. Gate: The 58-Rule Deterministic Audit & Multi-Viewport Verification
Run the audit checklist in [`references/anti-slop-58-rules.md`](references/anti-slop-58-rules.md) across the source code and rendered viewports (`1440px` desktop, `768px` tablet, `390px` mobile):
- Verify **0 banned tells** (no eyebrows/kickers, no gradient text, no purple-blue glows, no 3-card icon rows, no `01/02/03` index markers, no monospace cosplay, no headlines $> 2$ lines, no broken/missing image files).
- Open and inspect the rendered page in a real browser (or preview tool) at `1440px`, `768px`, and `390px`. Check that every generated Nano Banana asset loads cleanly, crops without clipping focal subjects, and maintains text legibility.

### 10. Polish & Delivery Report
Fix any findings from Step 9, then present a concise **Delivery Report**:
- **Art Direction & Idea:** Surface mode, Theme Paradigm, the **Idea Sentence** (and how it passes the Competitor Test), and **One Live Thing**.
- **Design Contract:** Path to `DESIGN.md`, `PRODUCT.md`, and `generations/refs/brand/style.md`.
- **High-Res Media Manifest:** Table of every generated Nano Banana / Omni Flash / Argon asset, its resolution (`2K`/`4K`), aspect ratio, file path, sidecar `.json` path, `response_id` (for future stateful edits), and total batch cost.
- **Audit Score:** Confirmation of `0 FAIL` across the 58 anti-slop rules at `1440px`, `768px`, and `390px`.

---

## Sub-Commands Vocabulary (`/ui <command>`)

You can invoke this skill for a full build or use its targeted Impeccable-style sub-commands on existing codebases (see [`references/commands-playbook.md`](references/commands-playbook.md) for full execution steps):

| Command | Category | What it does |
|---|---|---|
| `/ui init` | Contract | Interviews or scans the project to create `PRODUCT.md`, `DESIGN.md`, and `generations/refs/brand/style.md`. |
| `/ui document` | Contract | Reverse-engineers an existing codebase's tokens, typography, and rules into `DESIGN.md` and `style.md`. |
| `/ui craft [target]` | Build | Runs the full 10-Step Master Run (Art Direction + Batch Nano Banana 2K/4K Media Plan + Build + Audit). |
| `/ui visual-plan [target]` | Media OP | Audits a page's empty/weak visual slots, proposes a cohesive Batch Media Plan (2K/4K plates, panoramic dividers, Omni video loop), quotes once, and generates with Series Lock. |
| `/ui edit-asset <file>` | Media OP | Reads the `.json` sidecar of an existing generated asset and runs a stateful delta edit via `previous_interaction_id` or promotes a 1K draft to 2K/4K on Nano Banana 2.1 / Pro. |
| `/ui audit [target]` | Evaluate | Runs the 58 deterministic anti-slop rules + contrast, 2-line headline, frame, and asset integrity checks without editing code. |
| `/ui critique [target]` | Evaluate | Scores the interface against the 14-pass Awwwards & UX rubric and names the top 3 highest-leverage fixes. |
| `/ui normalize [target]` | Refine | Aligns drifted spacing, border-radii, font sizes, colors, and image treatments back to `DESIGN.md`. |
| `/ui polish [target]` | Refine | Final zero-defect pass: eliminates all detected AI tells, themes browser surfaces, optimizes image attributes, and re-runs `/ui audit` until 0 fails. |
| `/ui typeset [target]` | Enhance | Fixes typographic scale, pairing, measure (`65–75ch`), tracking, tabular numerals, and the 2-line headline rule. |
| `/ui colorize [target]` | Enhance | Replaces flat grey-on-color or generic palettes with `DESIGN.md` ground/ink/accent proportions and hue-tinted secondaries. |
| `/ui layout [target]` | Enhance | Fixes outer frame margins, eliminates huddled half-empty sections, and varies composition anchors across neighboring sections. |
| `/ui animate [target]` | Enhance | Adds the 4-part purposeful motion layer (signature move, staggered section entrances, control feedback, living media + reduced-motion fallback). |
| `/ui bolder [target]` | Adjust | Amplifies safe/timid UI: upgrades to Giant Statement scale, fuller color fields, and 4K full-bleed or panoramic Nano Banana plates. |
| `/ui quieter [target]` | Adjust | Strips visual noise, glowing borders, and competing accents into calm, high-craft precision (essential for `Operate` mode). |
| `/ui distill [target]` | Adjust | Removes redundant sections, nested cards, and filler copy down to the core argument. |
| `/ui harden [target]` | Fix | Production-readies all states (`hover`, `focus-visible`, `active`, `disabled`, `loading`, `empty`, `error`), keyboard nav, and `390px` thumb ergonomics. |
| `/ui overdrive [target]` | Enhance | Pushes visual ambition to gallery/experiment level: Gemini 4 Argon custom WebGL/GLSL shaders, scroll-pinned stages, and first-frame-to-video choreography. |

---

## Models & Pricing Reference

Always read the corresponding recipe in [`models/`](models/) before executing any API call. All calls use Google's **Interactions API** (`client.interactions.create`) via the official `google-genai` SDK.

| Role in UI / Frontend | Model | Model ID | Resolution & Key Specs | Standard Cost (Nov 2026) | Recipe |
|---|---|---|---|---|---|
| **Fast UI Drafts** | Nano Banana 2 Lite | `gemini-3.1-flash-lite-image` | `1K` only, sub-2s latency, 1–2 refs | ~$0.034 / image | [`models/nano-banana-2-lite.md`](models/nano-banana-2-lite.md) |
| **Standard 2K/4K UI & Panoramic Plates** | Nano Banana 2.1 | `gemini-nano-banana-2.1` | `1K`, `2K`, `4K`; ratios up to `21:9`, `4:1`, `1:4`, `8:1`, `1:8`; up to 14 refs | ~$0.034 (1K), ~$0.050 (2K), ~$0.113 (4K) | [`models/nano-banana-2.md`](models/nano-banana-2.md) |
| **Studio 2K/4K Hero & Multi-Ref Brand Fusion** | Nano Banana Pro | `gemini-3-pro-image` | `1K`/`2K` (same token cost!), `4K`; 14 refs (5 chars, 6 objects, 3 style refs) | ~$0.134 (1K/2K), ~$0.24 (4K) | [`models/nano-banana-pro.md`](models/nano-banana-pro.md) |
| **Hero-to-Video Muted Loops (3s–15s)** | Gemini Omni 1.2 Flash | `gemini-omni-1.2-flash` | 3–15s @ 24fps, `720p`/`1080p`/`4k`, natural-language starting-frame lock, extend up to 30s | ~$0.10 / second (720p) | [`models/gemini-omni-flash.md`](models/gemini-omni-flash.md) |
| **Fast UI Prototyping, SVGs & Ref Analysis** | Gemini 4 Hydrogen | `gemini-4-hydrogen` | 1M context, thinking (`low`/`medium`/`high`/`xhigh`), fast daily driver | $1.50/1M input, $7.50/1M output (Free tier in AI Studio) | [`models/gemini-4-hydrogen.md`](models/gemini-4-hydrogen.md) |
| **Fast Frontier Execution, 3D/SVGs & Copy** | Gemini 4 Neon | `gemini-4-neon` | 1M context, thinking (`low`/`medium`/`high`/`xhigh`), fast frontier completion | $3.00/1M input, $15.00/1M output | [`models/gemini-4-neon.md`](models/gemini-4-neon.md) |
| **Efficient Frontier 3D/Shaders & Storyboard** | Gemini 4 Argon | `gemini-4-argon` | 1M context, tunable thinking (`low`/`medium`/`high`), code visuals | $2/1M input, $10/1M output ($4/$20 Dec 1) | [`models/gemini-4-argon.md`](models/gemini-4-argon.md) |
| **Maximum-Depth Reasoning, 3D & GLSL Shaders** | Gemini 4 Carbon | `gemini-4-carbon` | 1M context, tunable thinking (`low`/`medium`/`high`), deepest verification | $2/1M input, $10/1M output ($4/$20 Dec 1) | [`models/gemini-4-carbon.md`](models/gemini-4-carbon.md) |

> **Pro Resolution Tip:** On `gemini-3-pro-image` (Nano Banana Pro), `1K` and `2K` both consume exactly `1,120` image output tokens (~$0.134). **Always request `"2K"` (or `"4K"` for giant retina heroes) on Nano Banana Pro** — requesting `"1K"` on Pro throws away 4x the pixel density for zero savings.

---

## Non-Negotiable House Rules

1. **Batch Cost Gate Before Paid Generation:** Present the complete **Batch Media Plan Table** (or single-call quote for one-off asset edits) with model IDs, resolutions, and expected USD total, and wait for explicit user approval before running paid API calls. Run approved generations **sequentially one at a time**, never in an unmonitored parallel flood.
2. **Real Brand Assets In, Cohesive Pixels Out:** Never describe an existing brand logo, founder face, or real product screenshot in words when a file exists in `generations/refs/` or the repo — pass the real image in `reference_images`.
3. **Hero-First Series Lock:** Never generate 6 independent section images with 6 unanchored prompts. Generate the Hero first, verify it, and pass the Hero image as a reference (plus `generations/refs/brand/style.md` verbatim) into every subsequent section image call so lighting, lens character, and color grading stay locked across the entire scroll.
4. **Save, Verify, Sidecar Log, Wire Into DOM:** Every generated file must be verified on disk and non-empty (`stat().st_size > 0`) before writing its matching `.json` sidecar (logging exact `model`, `prompt`, `reference_images`, `response_id`, `params`, `cost`, `created`, `approved_by_user`). Every generated UI image must be wired into the component/HTML with proper `alt`, `width`, `height`, and loading attributes.
5. **Zero AI Slop:** Enforce all 58 deterministic rules in [`references/anti-slop-58-rules.md`](references/anti-slop-58-rules.md). Removal of tells is only half the job — always replace removed ornaments with large, confident typography, real 2K/4K Series-Locked visuals, full section copy, and **One Live Thing**.

---

## Reference Library Map

| File | When to read it |
|---|---|
| [`references/design-contract.md`](references/design-contract.md) | Creating or reading `DESIGN.md`, `PRODUCT.md`, and `generations/refs/brand/style.md`; stack integration (Angular Signals/zoneless, React, Astro, Tailwind, GSAP). |
| [`references/art-direction-and-copy.md`](references/art-direction-and-copy.md) | Step 1–4: Subject Inventory, Competitor Test, One Live Thing, Two-Line Headline Arithmetic, Combinatorial Direction Matrix, and Operate/App-Screen rules. |
| [`references/nanobanana-visual-pipeline.md`](references/nanobanana-visual-pipeline.md) | Step 5–6: Batch Media Plan table, Photographer's Brief prompt formula, Negative-Space Safe Zones, Hero-First Series Lock, Panoramic ratios, Omni Flash video loops, Argon shaders/SVGs. |
| [`references/anti-slop-58-rules.md`](references/anti-slop-58-rules.md) | Step 7 & 9: The 58 deterministic anti-slop rules (`SLOP-01` to `SLOP-58`), Craft Floor verification, and exact code remediations. |
| [`references/commands-playbook.md`](references/commands-playbook.md) | Running any `/ui <sub-command>` (`audit`, `normalize`, `polish`, `typeset`, `colorize`, `layout`, `animate`, `bolder`, `quieter`, `distill`, `harden`, `overdrive`, `visual-plan`). |
| [`models/nano-banana-2.md`](models/nano-banana-2.md) | Calling Nano Banana 2.1 (`gemini-nano-banana-2.1`) for 1K/2K/4K & panoramic UI imagery. |
| [`models/nano-banana-pro.md`](models/nano-banana-pro.md) | Calling Nano Banana Pro (`gemini-3-pro-image`) for 2K/4K studio heroes, typography, & 14-ref fusion. |
| [`models/nano-banana-2-lite.md`](models/nano-banana-2-lite.md) | Calling Nano Banana 2 Lite (`gemini-3.1-flash-lite-image`) for rapid 1K composition drafts. |
| [`models/gemini-omni-flash.md`](models/gemini-omni-flash.md) | Calling Gemini Omni 1.2 Flash (`gemini-omni-1.2-flash`) for starting-frame-locked muted UI video loops (`3s`–`15s`). |
| [`models/gemini-4-hydrogen.md`](models/gemini-4-hydrogen.md) | Calling Gemini 4 Hydrogen (`gemini-4-hydrogen`) for fast daily-driver SVG/UI prototyping and multimodal reference analysis. |
| [`models/gemini-4-neon.md`](models/gemini-4-neon.md) | Calling Gemini 4 Neon (`gemini-4-neon`) for fast frontier end-to-end execution on complex interactive components and 3D visuals. |
| [`models/gemini-4-argon.md`](models/gemini-4-argon.md) | Calling Gemini 4 Argon (`gemini-4-argon`) for efficient frontier reasoning on SVGs, Three.js, GLSL shaders, and storyboard planning. |
| [`models/gemini-4-carbon.md`](models/gemini-4-carbon.md) | Calling Gemini 4 Carbon (`gemini-4-carbon`) for maximum reasoning depth on complex Three.js/WebGL scenes, GLSL shaders, and system verification. |

---

## Installation & Updating

Install directly via the `skills` CLI:

```bash
npx skills add AntonioCardenas/ui-nanobanana
```

Or manually clone into your agent's skills directory (the folder name `ui` registers the `/ui` slash command):

```bash
git clone https://github.com/AntonioCardenas/ui-nanobanana ~/.claude/skills/ui
```

**Updating (`/ui update`):**
1. Locate the folder this `SKILL.md` was loaded from.
2. If it is a git clone (`.git` exists), run `git pull`. Otherwise re-run `npx skills add AntonioCardenas/ui-nanobanana`.
3. Report the updated commits/changes to the user and remind them to restart their session if needed. Never touch the workspace's `DESIGN.md`, `PRODUCT.md`, or `generations/` folder during a skill update.

---

## Authentication & Security

- **API Key:** Reads `GEMINI_API_KEY` from the shell environment or a `.env` file at the workspace root (`set -a; source .env; set +a`). Never writes, logs, or commits `GEMINI_API_KEY`, and never creates or modifies `.env` files. In **Antigravity**, if `GEMINI_API_KEY` is absent, falls back cleanly to Antigravity's built-in `generate_image` tool for instant previews.
- **SDK:** Uses Google's official `google-genai` Python package (`python3 -c "import google.genai"`). Ask the user before installing if missing.
- **Network & File Scope:** HTTPS calls go strictly to `generativelanguage.googleapis.com`. File writes stay strictly inside the current project workspace (`DESIGN.md`, `PRODUCT.md`, project source/asset folders, and `generations/`).

