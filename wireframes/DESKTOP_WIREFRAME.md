# Desktop Wireframe (1200px+)

## Layout Overview

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│                      HEADER SECTION                         │
│              (Hero with Glass Background)                   │
│                                                             │
│              Style Stage Centered Title                     │
│              Description & GitHub Button                    │
│                                                             │
│            [Background Glow Effects + Animation]            │
│                                                             │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│ About  | Guidelines | Contribute | Files | Styles | Resources│
│            (Sticky Navigation with Underline Effect)        │
└─────────────────────────────────────────────────────────────┘

┌──────────────────────────┬──────────────────────────┐
│                          │                          │
│     SECTION 1            │     SECTION 2            │
│   (Glass Card)           │   (Glass Card)           │
│                          │                          │
│  • Title in Gold         │  • Title in Gold         │
│  • Content               │  • Content               │
│  • Links in Purple       │  • Links in Purple       │
│                          │                          │
│  Hover: Lift Up (-8px)   │  Hover: Lift Up (-8px)   │
│  Fade-in Animation       │  Fade-in Animation       │
│                          │                          │
└──────────────────────────┴──────────────────────────┘

┌──────────────────────────┬──────────────────────────┐
│                          │                          │
│     SECTION 3            │     SECTION 4            │
│   (Glass Card)           │   (Glass Card)           │
│                          │                          │
│  • Title in Gold         │  • Title in Gold         │
│  • Content               │  • Content               │
│  • Links in Purple       │  • Links in Purple       │
│                          │                          │
│  Hover: Lift Up (-8px)   │  Hover: Lift Up (-8px)   │
│  Fade-in Animation       │  Fade-in Animation       │
│                          │                          │
└──────────────────────────┴──────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│                                                             │
│                      FOOTER SECTION                         │
│                  (Glass Background)                         │
│                                                             │
│              Logo & Link Information                        │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

## Design Elements

| Element | Style | Properties |
|---------|-------|------------|
| Header | Glass morphism | `background: rgba(255,255,255,0.1)`, `backdrop-filter: blur(10px)`, `border-radius: 16px` |
| Sections | Glass cards | Same as header, plus animation fade-in & hover lift |
| Footer | Glass morphism | Same as header |
| Text | Hierarchy | H1/H2 in gold (#f0c95b), body in light gray |
| Accents | Interactive | Purple (#8e73ff) for links, glow effects |
| Layout | Grid | `grid-template-columns: repeat(2, 1fr); gap: 20px` |

## Animations

- **Fade-in:** Sections appear smoothly on page load (staggered 0.2s delays)
- **Hover:** Sections move up 8px with enhanced shadow
- **Transition:** All changes smooth over 0.3s
- **Glow:** Background has fixed blur glows (top-left blue, bottom-right purple)

