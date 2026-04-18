# Divi Layout Patterns

Common layout patterns and how to build them in Divi.

## Hero Patterns

### Fullwidth Hero with Centered Content

```
Section: Fullwidth, Fullscreen (optional)
├── Background: Image or Gradient
├── Row: Centered vertically and horizontally
│   └── Column: 2/3 width on desktop
│       ├── Text Module: Large headline (H1)
│       ├── Text Module: Subheadline
│       └── Button Module: Primary CTA
└── Scroll down indicator (optional): Blurb with arrow icon
```

**Settings:**
- Section: Fullwidth, Min-height: 100vh (optional)
- Row: Vertically centered
- Text: Large size (60-80px headline), contrasting colors

### Hero with Side-by-Side Content

```
Section: Fullwidth
├── Row: 2 columns (1/2 + 1/2)
│   ├── Column 1: Vertically centered
│   │   ├── Text Module: Headline
│   │   ├── Text Module: Description
│   │   └── Button Group: 2 buttons (primary + secondary)
│   └── Column 2:
│       └── Image Module: Hero image/illustration
└── Optional: Bottom wave divider
```

### Hero with Overlapping Elements

```
Section: Regular, Custom padding
├── Row: 2 columns with different vertical alignments
│   ├── Column 1: Bottom aligned
│   │   └── Text Modules + Buttons
│   └── Column 2: Top aligned
│       └── Image Module
└── Scroll effects on image (optional)
```

## Content Section Patterns

### Zigzag Content (Alternating)

```
Section 1: White background
└── Row: 2 columns
    ├── Column 1: Image
    └── Column 2: Text content

Section 2: Light gray background
└── Row: 2 columns
    ├── Column 1: Text content (reversed order)
    └── Column 2: Image
```

**Tip:** Use "Row → Column Settings → Column Order" to reverse on mobile

### Three-Column Features

```
Section
└── Row: 3 columns (1/3 + 1/3 + 1/3)
    ├── Column 1:
    │   └── Blurb Module (Icon + Title + Text)
    ├── Column 2:
    │   └── Blurb Module
    └── Column 3:
        └── Blurb Module
```

**Variations:**
- Icons on top (default)
- Icons on left (Blurb layout setting)
- Circle icons (Icon background color + border-radius)

### Four-Column Grid

```
Section
├── Row: 4 columns (1/4 + 1/4 + 1/4 + 1/4)
│   └── Blurb/Image/Text modules in each
```

**Responsive:** Automatically stacks to 2x2 on tablet, 1 column on mobile

## CTA Patterns

### Simple CTA Bar

```
Section: Background color
└── Row: 2 columns (2/3 + 1/3)
    ├── Column 1:
    │   └── Text Module: CTA text
    └── Column 2:
        └── Button Module: Right aligned
```

### CTA with Background Image

```
Section: Background image + overlay
└── Row: Centered
    └── Column: 2/3 width
        ├── Text Module: Headline
        ├── Text Module: Description
        └── Button Group: Multiple CTAs
```

## Testimonial Patterns

### Single Testimonial

```
Section
└── Row: Centered
    └── Column: 2/3 width
        └── Testimonial Module: Quote, Author, Image
```

### Testimonial Grid

```
Section
└── Row: 3 columns
    ├── Column 1: Testimonial Module
    ├── Column 2: Testimonial Module
    └── Column 3: Testimonial Module
```

### Testimonial Slider

```
Section
└── Row: Fullwidth
    └── Column: 1 column
        └── Slider Module: Fullwidth, Auto-animate
            └── Each slide: Testimonial layout
```

## Portfolio/Showcase Patterns

### Portfolio Grid

```
Section
└── Row: Fullwidth
    └── Column
        └── Portfolio Module: Grid layout
            ├── Categories enabled
            └── 4-6 items
```

### Project Showcase (Alternating)

```
Section 1
└── Row: 2 columns
    ├── Column 1: Image (Project screenshot)
    └── Column 2: Project details (Text + Button)

Section 2
└── Row: 2 columns (reversed)
    ├── Column 1: Project details
    └── Column 2: Image
```

## Pricing Patterns

### Three-Tier Pricing

```
Section
└── Row: 3 columns (1/3 + 1/3 + 1/3)
    ├── Column 1: Pricing Table Module
    ├── Column 2: Pricing Table Module (Featured/Highlighted)
    └── Column 3: Pricing Table Module
```

**Settings:**
- Middle column: Offset transform (lift up), different background color
- Featured column: "Featured" badge

### Comparison Table

```
Section
└── Row
    └── Column
        └── Pricing Table Module: Side-by-side comparison
```

## Team/About Patterns

### Team Grid

```
Section
└── Row: 4 columns (1/4 x 4)
    └── Team Member Module in each column
        ├── Photo
        ├── Name
        ├── Position
        └── Social links
```

**Responsive:** 4 cols → 2 cols → 1 col

### About with Stats

```
Section
└── Row: 4 columns
    ├── Column 1: Blurb (Icon + Number + Label)
    ├── Column 2: Blurb
    ├── Column 3: Blurb
    └── Column 4: Blurb
```

## Blog/Content Patterns

### Latest Posts Grid

```
Section
└── Row: Fullwidth
    └── Column
        └── Blog Module: Grid layout, 3 posts
```

### Featured Post + List

```
Section
└── Row: 2 columns (2/3 + 1/3)
    ├── Column 1: Blog Module: Fullwidth (1 featured)
    └── Column 2: Blog Module: List (3 recent)
```

## Contact Patterns

### Contact Page (Standard)

```
Section 1: Contact Form
└── Row: 2 columns (2/3 + 1/3)
    ├── Column 1:
    │   ├── Text Module: Page title
    │   └── Contact Form Module
    └── Column 2:
        ├── Blurb: Address
        ├── Blurb: Phone
        └── Blurb: Email

Section 2: Map
└── Row: Fullwidth
    └── Column
        └── Map Module
```

### Split Contact Layout

```
Section
└── Row: 2 columns (1/2 + 1/2)
    ├── Column 1:
    │   ├── Text Module: Contact info
    │   └── Social Media Follow Module
    └── Column 2:
        └── Contact Form Module
```

## Footer Patterns

### Four-Column Footer

```
Footer Section (via Theme Builder)
└── Row: 4 columns
    ├── Column 1: Logo + About text
    ├── Column 2: Quick Links (Menu)
    ├── Column 3: Contact Info
    └── Column 4: Newsletter signup
```

### Minimal Footer

```
Footer Section
└── Row: Centered
    └── Column
        ├── Social Media Follow: Centered
        └── Text Module: Copyright
```

## Advanced Patterns

### Asymmetric Grid

```
Section
├── Specialty Section Layout
│   ├── Left: 1/3 width
│   │   └── Tall content (image or text)
│   └── Right: 2/3 width
│       └── Multiple rows/modules
```

### Sticky Content

```
Section
└── Specialty Section
    ├── Left: 1/4 width, Sticky
    │   └── Navigation/TOC
    └── Right: 3/4 width
        └── Scrollable content
```

### Fullwidth with Constrained Content

```
Section: Fullwidth background
└── Row: Centered, Max-width: 1080px
    └── Column
        └── Content modules
```

**Use for:** Parallax sections, colored backgrounds with centered content

## Animation Patterns

### Scroll-Reveal Elements

1. Add animation to modules: "Slide In Bottom"
2. Set animation delay for staggered effect
3. Configure: Duration, Delay, Easing

### Hover Effects

- Image modules: Zoom on hover
- Blurbs: Icon color change
- Buttons: Background/border transition

## Responsive Considerations

### Mobile-First Adjustments

1. **Stack columns**: Most multi-column layouts should stack
2. **Reduce font sizes**: Desktop 60px → Mobile 36px
3. **Hide decorative elements**: Parallax, animations on mobile
4. **Adjust spacing**: Less padding on mobile

### Breakpoint Behavior

| Desktop | Tablet | Mobile |
|---------|--------|--------|
| 4 columns | 2 columns | 1 column |
| Side-by-side | Stacked | Stacked |
| Full animations | Reduced | Minimal |
| Large text | Medium | Small |

## Best Practices

1. **Consistent spacing**: Use same section padding throughout
2. **Visual hierarchy**: Clear headline → subhead → body text sizes
3. **White space**: Don't crowd elements
4. **Color consistency**: Use global colors
5. **Mobile testing**: Check all breakpoints
6. **Load optimization**: Optimize images, use WebP
