# Presentation Microsite Patterns

## Recommended architecture

```text
app/
  page.tsx
components/
  sections/
    hero-section.tsx
    problem-section.tsx
    insight-section.tsx
    solution-section.tsx
    proof-section.tsx
    highlight-section.tsx
    final-cta-section.tsx
  ui/
content/
  site.json
  sections/*.mdx
lib/
  motion.ts
  media.ts
public/
  videos/
  images/
```

## Section patterns

### Hero
Goal: establish mood and thesis quickly.
Use:
- strong typography
- one key visual
- short motion intro
- one sharp subheading

### Sticky explanation
Goal: explain a process or system gradually.
Use:
- sticky visual panel
- step text column
- active-state transitions by scroll position

### Metric reveal
Goal: make numbers feel earned.
Use:
- delayed count-up
- comparison framing
- concise annotation

### Case strip
Goal: show proof without clutter.
Use:
- horizontally scrollable cards on mobile
- concise outcome-oriented titles
- image/video only if it adds signal

### Highlight moment
Goal: create the memory anchor.
Use one dominant move:
- giant statistic
- product montage
- cinematic Remotion clip
- animated system diagram

## Motion heuristics

Use motion when it improves one of these:
- focus
- causality
- sequence
- scale
- emotional emphasis

If motion does not improve one of those, cut it.

## Responsive rule

Design desktop and mobile as separate experiences sharing one narrative. Do not merely shrink desktop.

## Performance rule

Prefer:
- compressed MP4/WebM
- poster images
- lazy-loaded heavy media
- CSS transforms over layout-thrashing animation

## Stack choices

### Default
- Next.js
- Tailwind
- Framer Motion

### Add GSAP when
- timeline orchestration is complex
- multiple synchronized elements depend on scroll progress

### Add Remotion when
- a cinematic sequence is easier to pre-render than animate live
- the same segment should be reused in social/video output
