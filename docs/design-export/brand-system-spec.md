---
page: Virginia Perpetua
kind: page
source: Brand-System-Spec.dc.html
slug: brand-system-spec
---

# Virginia Perpetua

Emerging full-stack engineer & IT graduate — Melbourne, Australia. Prepared as a governing reference for the personal brand ecosystem (website, resume, and future work).

## 1. Executive Creative Direction

Virginia is finishing an IT degree while running daily operations at a gelato store — the rare early-career candidate who has already managed a real, numbers-driven environment. The brand's job is to make one thing obvious in under a minute: she notices operational friction and builds working software for it , and she is now pointing that same instinct at full-stack engineering and AI/automation.

Visual direction: a flat, gridded, editorial system — not a decorative "creative portfolio" and not a dry corporate resume site. Modernist's architecture (visible grid, strong rules, flush-left type, zero ornament) reads as systems-thinking made visible, which is exactly the story: an operator who organises chaos into clear structure. The accent is spent on hierarchy and a small number of high-conviction moments — the gelato case study's poster statement, primary actions, and the section that names her future direction — never as background decoration.

## 2. Personal Brand → Visual Design Translation

## 3. Design Principles

## 4. Colour System

Primitives are Modernist's own tonal-ramp structure, retuned to a light-purple accent. Full ramps below, at swatch size:

Semantic roles map onto these ramps as follows:

Semantic mapping used across the site:

Dark mode: ground drops to neutral-900 (#2d2b2b), surface to neutral-800, text inverts to neutral-100; accent shifts one step brighter ( --color-accent-400 #b494f7) to hold contrast on dark ground; dividers become 25% white-mix. Same ramps, same rules, inverted assignment — not a CSS filter-invert.

## 5. Typography System

Single-family system by design: Archivo for both heading and body ( --font-heading , weight 800; --font-body , weight 400), plus a system monospace stack for metadata. Archivo's grotesque, slightly architectural letterforms already carry the "structured but human" tone the brief calls for — a second display face would fight the grid rather than reinforce it.

Rationale: one grotesque family kept consistent end-to-end signals engineering discipline; the monospace layer is reserved strictly for system-like metadata (never body copy), so it reads as "operational label," not "code aesthetic."

## 6. Spacing System

Semantic additions layered on top for page-level rhythm: --space-section 96px desktop / 56px mobile; --space-page-gutter 48px desktop / 20px mobile; --content-width-reading 680px; --content-width-project 920px; --content-width-max 1200px.

## 7. Layout & Grid System

12-column grid on desktop, 24px gap, max content width 1200px, gutters scale with viewport. The grid stays visible — thin dividers mark column/section boundaries on the homepage and case study, per Modernist's architectural direction.

## 8. Shape, Surface & Elevation

--radius-* is 0 everywhere — no rounded corners, per system. Surfaces are separated by the 2px .hr rule and by fill ( --color-surface vs --color-bg ), not by shadow. Elevation ( --shadow-sm/md/lg ) is reserved for the one truly "floating" object in the whole system: the contact-form card and modal dialogs. Cards otherwise sit flush in the grid with a divider, never a shadow.

## 9. Motion System

Signature behaviour: project cards respond to hover by raising text weight and running the accent underline under the title — no scale/tilt/shadow-pop. Section reveals fade + rise 8px, staggered by child, once, never re-triggered on re-scroll. All motion respects prefers-reduced-motion : reveals render in final state instantly, hover fills still apply (they're not "motion" for accessibility purposes).

## 10. Complete Design Token Architecture

Three tiers, consistent with Modernist's own token file:

Naming: --{category}-{role}-{variant?} , all kebab-case, directly portable to Figma Variables (category/role/variant collections) and Tailwind ( colors.action.primary , etc).

## 11. Component Library

## 12. Page-by-Page Design System

## 13. Project & Case Study System

Three depth tiers so the system scales as new work appears:

## 14. Resume / CV System

Print-first, ATS-conscious: single column, no tables-as-layout, real <h1>–<h3> hierarchy, Archivo throughout (renders as a clean sans if unavailable — no glyph loss), accent used only for the name rule and section-label colour, both of which survive as pure black in grayscale printing.

## 15. Responsive Rules

## 16. Accessibility Rules

## 17. Design System Governance

## 18. Implementation Notes

## 19. Final Visual Direction Summary

A flat, gridded, Archivo-set system in ink on warm off-white, with one deliberate accent spent only on hierarchy and conviction. The gelato tool leads every page it can — proof that this is someone who turns a shift on the floor into a working system. Everything else — the retake, the languages, the curiosity about AI — sits inside that same disciplined structure, visible but never louder than the evidence.

## Visual

- Long-form documentation canvas; dense token/swatch documentation stacked vertically.
- Same purple accent ramp and Archivo system as the site pages; zero radius throughout.
