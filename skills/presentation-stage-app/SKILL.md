---
name: presentation-stage-app
description: Build or plan a slide-like stage presentation web app for talks, demos, internal reviews, keynote-style decks, product walkthroughs, training sessions, and live presentations that need to look better than PowerPoint while remaining controllable on stage. Use when the user wants a frontend presentation with slide navigation, keyboard control, speaker flow, polished transitions, component-based layouts, or optional Remotion video segments.
---

# Presentation Stage App

Build a stage-controlled presentation app: linear, crisp, presenter-friendly, and visually superior to PPT. Optimize for pacing, legibility, reliability, and live delivery.

## Workflow

1. Confirm the presentation is primarily linear.
2. Design the deck as a sequence of scenes.
3. Pick a lightweight control model.
4. Build reusable slide primitives.
5. Add motion that supports speaking rhythm.
6. Add export or recording paths if needed.

## 1. Fit check

Choose this skill when the user needs:
- keynote-style web presentation
- on-stage demo flow
- slide navigation with keyboard or clicker behavior
- speaker notes or presenter mode
- a deck-like experience with better UI/UX than PPT

If the user wants free exploration, long-form storytelling, or web sharing first, prefer `presentation-microsite` instead.

## 2. Core stack

Default choices:
- React or Next.js
- Tailwind CSS
- Framer Motion
- optional MDX / structured content
- optional Remotion for intro/outro or pre-rendered animated segments

Good alternative frameworks when the user explicitly wants them:
- Slidev
- reveal.js
- Spectacle

Prefer custom React/Next.js when the request needs brand-specific UI, embedded app states, or custom presenter features.

## 3. Model the presentation as scenes

Do not think in office-slide habits. Think in scenes with a speaking purpose:
- title / premise
- context
- problem
- proposal
- evidence
- demo
- conclusion

For each scene, define:
- speaker intent
- maximum 1 primary visual idea
- reveal sequence
- navigation behavior
- time budget

## 4. Use slide primitives

Build reusable primitives such as:
- `TitleSlide`
- `StatementSlide`
- `SplitVisualSlide`
- `MetricSlide`
- `TimelineSlide`
- `DemoSlide`
- `QuoteSlide`
- `ClosingSlide`

Keep a consistent spacing, typography, and reveal model. A stage app feels premium when the system is coherent, not when every slide is unique.

## 5. Motion rules

Use motion to support the speaker:
- progressive reveal
- enter/exit transitions
- emphasis pulses
- controlled content sequencing
- demo framing transitions

Avoid:
- complex scroll dependencies
- distracting ambient motion
- unreadable full-screen video backgrounds
- transitions that delay pacing

Every slide should remain readable in its resting state.

## 6. Controls and presenter UX

A good stage app usually needs:
- arrow-key navigation
- jump-to-scene support
- progress indicator
- stable aspect ratio handling
- optional notes view
- fallback for browser zoom / projector issues

If the user mentions live delivery, reliability beats novelty.

## 7. Remotion usage

Use Remotion selectively for:
- cold open video
- interstitials
- polished demo bumpers
- ending recap clip
- reusable promo exports

Do not force every animated slide into a video. Live slides should stay interactive where helpful.

## 8. Delivery standard

A strong stage app deliverable usually includes:
- scene inventory
- reusable slide system
- keyboard navigation
- consistent transition language
- responsive presenter-safe layout
- asset preload strategy
- speaker-tested pacing

When planning or implementing, include:
- slide taxonomy
- route or state model
- content source strategy
- presenter controls
- export / recording plan if needed

## 9. Common mistakes

Flag these fast:
- rebuilding boring PPT slide patterns in React
- placing too much copy on screen
- making each slide a new visual language
- over-animating transitions
- relying on network-fetched assets during live talks
- forgetting projector-safe contrast and font size

## 10. Read more only when needed

If the task needs deeper examples, read:
- `references/patterns.md` for scene patterns, control models, and layout rules
- `references/project-brief-template.md` for discovery questions before implementation
