---
name: divi-website-creator
version: 5.0
description: Build modern Divi 5 WordPress websites from mockups, HTML files, or design descriptions. Uses Divi 5+ features: Group modules, Group Carousels, News Variable Manager for global variables, custom post types, and advanced responsive controls.
---

# Divi Website Creator

Build professional WordPress websites using Divi 5.0+ with modern features.

## Overview

This skill uses **Divi 5.0+** modern features to build WordPress websites:

- **Group & Group Carousel modules** for dynamic content organization
- **News Variable Manager** for centralized global variables (fonts, colors, responsive values)
- Modern **custom post types** and **template parts**
- Advanced **module grouping** and **conditional display**
- Better **responsive controls** with per-module breakpoint settings

## Prerequisites

- WordPress installation
- **Divi 5.0+** theme installed and activated
- **News Variable Manager** plugin (recommended for Divi 5 variable system)
- Access to Divi Builder (Visual Builder or Backend Builder)
- Understanding of global variables system in Divi 5

## Divi 5 Key Features

### Group Modules
- Groups organize multiple modules
- Enables consistent styling across related modules
- Can be styled independently from containing module
- Use for: CTAs, feature sets, testimonial rows

### Group Carousel
- Carousel-style module groups
- Auto-plays or manual navigation
- Great for featured content, portfolios, testimonials
- Each item can have its own settings

### News Variable Manager
- Centralized control for fonts, colors, spacing, responsive values
- Update once, changes everywhere
- Per-variable breakpoint settings
- Recommended for: brand colors, font sizes, padding/margin scales

### Module Groups in Sections
- Groups of modules can be styled together
- Use for consistent section layouts
- Enable "group styling" for unified appearance

## Core Group Types

| Group | Use Case | Example |
|-------|-------|---------|
| **CTA Group** | Call-to-action modules | Button + Icon + Text group |
| **Features Group** | Feature showcase | 3-6 blurb modules in group |
| **Testimonial Group** | Testimonials | Group of quote modules |
| **Product Showcase** | Product grid | Group of Product modules |
| **Content Group** | Blog/portfolio | Group of Blog/Portfolio items |

## Workflow with Divi 5

1. **Analyze Input**: HTML file, mockup image, or design description
2. **Plan Structure**: Define section groups and rows
3. **Setup Global Variables**: Configure News Variable Manager for fonts, colors
4. **Build with Groups**: Use Group modules to organize content
5. **Apply Group Styling**: Unified appearance across related modules
6. **Configure Group Carousels**: For featured content sections
7. **Configure Responsive**: Use News Variable Manager for breakpoint-specific values
8. **Test & Polish**: Verify all breakpoints and animations
9. **Export**: Save groups to Library for reuse

## Updated Structure Reference

```
Page
├── Theme Builder: Header/Footer
├── Section
│   ├── Group (CTA/Features/Testimonial/Product)
│   │   ├── Module
│   │   ├── Module
│   │   └── Module
│   └── Row
│       ├── Column
│       │   └── Group Carousel
│       │       ├── Item
│       │       ├── Item
│       │       └── Item
└── Section
```

## Global Variables System

Configure in **News Variable Manager**:

### Variables to create:

**Colors:**
- `Primary:0` - Main brand color
- `Primary:1` - Lighter variant
- `Accent:0` - Secondary accent color
- `Background:0` - Main background
- `Text:0` - Primary text
- `Text:1` - Secondary text

**Fonts:**
- `Font:Headline` - H1/H2 font
- `Font:Body` - Body text font
- `Font:Accent` - Accent font (optional)

**Spacing:**
- `Spacing:Padding` - Section padding
- `Spacing:Margin` - Module margin
- `Spacing:Gap` - Between columns/rows

**Responsive:**
- Set per-variable breakpoint values
- Example: Font size scaling (64px → 48px → 32px)

## Resources

- [Divi 5 Documentation](https://www.elegantthemes.com/documentation/divi/)
- [Divi 5 Global Variables](https://www.elegantthemes.com/documentation/divi/variables/)
- [Module Groups Reference](references/divi-modules.md)
- [Divi 5 Variable Manager Guide](references/divi-5-variables.md)
- [Layout Patterns](references/layout-patterns.md)
- [Workflows](references/workflows.md)
