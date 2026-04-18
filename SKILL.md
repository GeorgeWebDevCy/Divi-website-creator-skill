---
name: divi-website-creator
description: Build Divi-based WordPress websites from mockups, HTML files, or design descriptions. Use when the user wants to create a WordPress website using the Divi theme, convert designs/mockups into Divi layouts, or build custom Divi pages from scratch. Supports HTML/CSS to Divi conversion, layout creation, module configuration, and responsive design implementation.
---

# Divi Website Creator

Build professional WordPress websites using the Elegant Themes Divi theme from mockups, HTML files, or design descriptions.

## Overview

This skill enables AI agents to:
1. Convert HTML mockups into Divi layouts
2. Create custom Divi pages from scratch
3. Configure Divi modules and settings
4. Implement responsive designs
5. Export/import Divi layouts

## Prerequisites

- WordPress installation
- Divi theme installed and activated
- Access to Divi Builder (Visual Builder or Backend Builder)

## Quick Start

### From HTML Mockup

1. Analyze the HTML structure (see [references/html-analysis.md](references/html-analysis.md))
2. Map HTML elements to Divi modules (see [references/module-mapping.md](references/module-mapping.md))
3. Create the layout using Divi Builder
4. Configure responsive breakpoints

### From Design Description

1. Identify layout patterns (see [references/layout-patterns.md](references/layout-patterns.md))
2. Select appropriate Divi modules
3. Configure colors, fonts, and spacing
4. Build sections, rows, and modules

## Divi Structure Reference

```
Page/Section
├── Section (Fullwidth / Regular / Specialty)
│   ├── Row (Column layout)
│   │   ├── Column
│   │   │   └── Module (Text, Image, Blurb, etc.)
│   │   └── Column
│   │       └── Module
│   └── Row
└── Section
```

## Core Modules

| Module | Use Case |
|--------|----------|
| **Text** | Headlines, paragraphs, basic content |
| **Image** | Photos, graphics, banners |
| **Blurb** | Icon + title + text combos |
| **Button** | CTAs, links, actions |
| **Slider** | Image galleries, carousels |
| **Testimonial** | Customer quotes, reviews |
| **Contact Form** | Lead capture, inquiries |
| **Pricing Table** | Product/service pricing |
| **Portfolio** | Project showcases |
| **Blog** | Post listings, recent articles |

## Responsive Breakpoints

- **Desktop**: > 981px
- **Tablet**: 768px - 980px
- **Mobile**: < 768px

## Workflow

1. **Analyze Input**: HTML file, mockup image, or design description
2. **Plan Structure**: Sections → Rows → Columns → Modules
3. **Create Layout**: Use Divi Builder to build page
4. **Configure Settings**: Colors, fonts, spacing, animations
5. **Test Responsive**: Check all breakpoints
6. **Export Layout**: Save for reuse (optional)

## Advanced Features

- **Custom CSS**: Add via Module → Advanced → Custom CSS
- **Global Defaults**: Set site-wide colors/fonts in Theme Customizer
- **Divi Library**: Save reusable sections/modules
- **Theme Builder**: Create custom headers/footers/templates

## Resources

- [Divi Documentation](https://www.elegantthemes.com/documentation/divi/)
- [Module Reference](references/divi-modules.md)
- [Layout Patterns](references/layout-patterns.md)
- [Common Workflows](references/workflows.md)
