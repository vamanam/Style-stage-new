# Mobile Wireframe (375px)

## Layout Overview

```
┌─────────────────────────────────┐
│                                 │
│      HEADER SECTION             │
│   (Hero with Glass BG)          │
│                                 │
│   Style Stage (Centered)        │
│   Description                   │
│   GitHub Button                 │
│                                 │
│  [Background Glow]              │
│                                 │
└─────────────────────────────────┘

┌─────────────────────────────────┐
│  Home | About | Guidelines | ... │
│   (Responsive Navigation)       │
└─────────────────────────────────┘

┌─────────────────────────────────┐
│                                 │
│      SECTION 1                  │
│    (Glass Card - Full Width)    │
│                                 │
│   • Title in Gold               │
│   • Content Paragraph           │
│   • Links in Purple             │
│                                 │
│   Fade-in Animation             │
│   Hover: Lift Up                │
│                                 │
└─────────────────────────────────┘

┌─────────────────────────────────┐
│                                 │
│      SECTION 2                  │
│    (Glass Card - Full Width)    │
│                                 │
│   • Title in Gold               │
│   • Content Paragraph           │
│   • Links in Purple             │
│                                 │
│   Fade-in Animation             │
│   Hover: Lift Up                │
│                                 │
└─────────────────────────────────┘

┌─────────────────────────────────┐
│                                 │
│      SECTION 3                  │
│    (Glass Card - Full Width)    │
│                                 │
│   • Title in Gold               │
│   • Content Paragraph           │
│   • Links in Purple             │
│                                 │
│   Fade-in Animation             │
│   Hover: Lift Up                │
│                                 │
└─────────────────────────────────┘

┌─────────────────────────────────┐
│                                 │
│      SECTION 4                  │
│    (Glass Card - Full Width)    │
│                                 │
│   • Title in Gold               │
│   • Content Paragraph           │
│   • Links in Purple             │
│                                 │
│   Fade-in Animation             │
│   Hover: Lift Up (Touch)        │
│                                 │
└─────────────────────────────────┘

┌─────────────────────────────────┐
│      FOOTER SECTION             │
│    (Glass Background)           │
│   Logo & Link Information       │
└─────────────────────────────────┘
```

## Mobile-Specific Adjustments

| Element | Mobile Style | Changes from Desktop |
|---------|--------------|----------------------|
| Layout | Single column | 1 column instead of 2 |
| Sections | Full width | Padding adjusted for small screens |
| Header | Responsive text | Font sizes use clamp() for fluid scaling |
| Navigation | Stacked/Scrollable | May stack vertically on very small screens |
| Spacing | Reduced padding | 20px padding instead of larger desktop values |
| Text | Optimized sizing | H1: 18px-36px, body: 16px |
| Glass effect | Same styling | Consistent glass morphism across all sizes |

## Touch Interactions

- Tap sections for hover-like effect (via `:active` or `:focus`)
- Smooth scrolling between sections
- No hover animations on touch (CSS handles via media queries)
- Full-width content for easier thumb interaction

## Breakpoint Strategy

```scss
// Default: Mobile first
main {
  display: grid;
  grid-template-columns: 1fr; // Single column
  gap: 20px;
  padding: 1rem;
}

// Tablet & Desktop
@media (min-width: 768px) {
  main {
    grid-template-columns: repeat(2, 1fr); // Two columns
    padding-top: 6vh;
    padding-bottom: 5vh;
  }
}
```

