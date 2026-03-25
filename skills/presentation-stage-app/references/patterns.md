# Presentation Stage App Patterns

## Recommended architecture

```text
app/
  present/[deck]/page.tsx
components/
  deck/
    deck-shell.tsx
    presenter-view.tsx
    progress-bar.tsx
  slides/
    title-slide.tsx
    statement-slide.tsx
    split-visual-slide.tsx
    metric-slide.tsx
    timeline-slide.tsx
    demo-slide.tsx
content/
  deck.json
lib/
  navigation.ts
  transitions.ts
  preload.ts
public/
  media/
```

## Scene patterns

### Title slide
Use one thesis, one support line, one focal visual.

### Statement slide
Use one strong claim plus one supporting proof point.

### Split visual slide
Use text on one side and product/media/diagram on the other. Keep hierarchy obvious.

### Metric slide
Use one number family only. Avoid dashboards on stage.

### Timeline slide
Reveal steps progressively instead of rendering the entire process at once.

### Demo slide
Frame the demo clearly:
- what to look at
- what changed
- why it matters

### Closing slide
End with one memorable line and one next action.

## Navigation models

### Index-based
Use when the deck is small and strictly linear.

### Scene-id based
Use when deep links, jump menus, or presenter shortcuts matter.

Prefer scene-id based routing when the deck may grow.

## Presenter notes

If notes are needed, keep them out of the audience DOM when possible. Treat notes as a separate presenter surface or hidden panel.

## Reliability rules

Prefer:
- local/static assets
- preload for large images or video needed in early scenes
- safe font sizes
- high contrast
- keyboard-first controls

Avoid depending on flaky live network calls during a talk.
