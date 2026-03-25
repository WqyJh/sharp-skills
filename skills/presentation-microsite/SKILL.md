---
name: presentation-microsite
description: Build or plan a narrative presentation microsite for launches, demos, reports, investor stories, annual reviews, case studies, landing pages, scrollytelling pages, and interactive showcase websites that should go beyond slide decks. Use when the user wants a polished frontend presentation website with strong UI/UX, scroll-driven storytelling, immersive sections, responsive behavior, presenter mode, or Remotion-assisted video segments.
---

# Presentation Microsite

Build a narrative microsite, not a web-wrapped slide deck. Optimize for story flow, visual polish, interaction quality, and post-meeting shareability.

## Workflow

1. Classify the request.
2. Define the narrative arc.
3. Choose the stack.
4. Design the section system.
5. Implement motion and media deliberately.
6. Add presenter mode only if it helps.
7. Ship a web-first experience.

## 1. Classify the request

Choose this skill when the user wants any of these:
- scrollytelling
- narrative microsite
- campaign page
- launch page
- annual report page
- investor or strategy story page
- interactive demo website
- a website that replaces or outclasses PPT

Do **not** default to slide metaphors. Treat the page as a directed experience with a beginning, progression, highlight moment, and ending.

## 2. Define the narrative arc

Before building, lock the story into 5-7 beats:
- opening hook
- context or problem
- insight or opportunity
- solution or system
- proof: metrics, cases, demos
- peak moment
- conclusion / CTA

If the user gives raw materials only, propose this structure explicitly instead of mirroring their outline blindly.

## 3. Choose the stack

Default stack:
- Next.js
- Tailwind CSS
- Framer Motion
- MDX or JSON content layer
- Remotion only for pre-rendered video segments or hero loops

Add only when justified:
- GSAP ScrollTrigger for complex scroll choreography
- Lenis for smoother scrolling feel
- Three.js / React Three Fiber only when 3D materially improves the story

Prefer the simplest stack that can deliver the desired effect. Most projects do **not** need heavy 3D.

## 4. Design the section system

Use a section model like this:
- `HeroSection`
- `ProblemSection`
- `InsightSection`
- `SolutionSection`
- `ProofSection`
- `HighlightSection`
- `FinalCTASection`

For each section, define:
- narrative goal
- primary visual
- motion behavior
- mobile fallback
- presenter-mode behavior if any

Keep content data-driven. Prefer content files, MDX, or structured JSON over hard-coded copy inside components.

## 5. Motion rules

Use motion to direct attention, not to show off.

Prefer:
- staged reveals
- sticky sections
- subtle parallax
- number count-up
- diagram progression
- before/after transitions
- media crossfades

Avoid:
- constant floating motion everywhere
- long blocking animations
- scroll-jacking that fights user input
- multiple competing focal points
- autoplay audio

If a section is hard to understand without animation, make sure it still has a static fallback state.

## 6. Remotion usage

Use Remotion for:
- opening film
- product feature montage
- background loops
- data highlight sequences
- recap / ending video
- short exportable social clips

Do **not** use Remotion as the entire site framework. Treat it as a media production layer that feeds the microsite.

## 7. Presenter mode

Add presenter mode only when the site must also work for live talks.

Presenter mode should usually provide:
- full-screen stage layout
- section-by-section navigation
- keyboard shortcuts
- clean URL state
- optional notes pane
- hidden chrome / minimal distractions

If the user mainly wants asynchronous viewing, keep presenter mode lightweight.

## 8. Delivery standard

A good microsite deliverable usually includes:
- clear story arc
- responsive layout
- polished hero
- 1-2 memorable interaction patterns
- fast loading media strategy
- accessible typography and contrast
- shareable deployment target

When proposing an implementation plan, include:
- route structure
- content model
- component map
- animation strategy
- media pipeline
- deployment recommendation

## 9. Common mistakes

Call these out early:
- turning the page into vertical slides
- overusing animation without information gain
- ignoring mobile layout until the end
- hard-coding copy and data into JSX
- using 3D for ego instead of clarity
- shipping giant videos with no fallback

## 10. Read more only when needed

If the task requires deeper structure or examples, read:
- `references/patterns.md` for architecture, section patterns, and animation heuristics
- `references/project-brief-template.md` for a reusable discovery and planning template
