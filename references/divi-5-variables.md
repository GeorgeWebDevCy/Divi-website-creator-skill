# Divi 5 Variable Manager Guide

The **News Variable Manager** plugin (required for proper Divi 5 variable system) allows centralized control over fonts, colors, and responsive values across your site.

## Setup News Variable Manager

### Step 1: Install Plugin

1. WordPress Admin → Plugins → Add New
2. Search "News Variable Manager"
3. Install & Activate
4. Go to News → Variable Manager

### Step 2: Create Variables

**Colors:**

```
Colors
├── Primary:0 (Main brand color)
│   ├── Default: #E40221 (Divi Red)
│   ├── Breakpoint values:
│   │   ├── >980px: #E40221
│   │   ├── 768px: #d6021b
│   │   └── <768px: #b90215
│   └── Usage: Assign to module background color
│
├── Primary:1 (Lighter variant)
│   └── Value: HSLA(0,100%,95%)
│
├── Accent:0 (Secondary accent)
│   └── Value: #279FE9 (Divi Blue)
│
├── Background:0 (Main background)
│   ├── Value: #FFFFFF
│   └── Breakpoint values: White on desktop
│
└── Background:1 (Secondary background)
    └── Value: #F7F8FA (Light gray)

Colors
├── Text:0 (Primary text)
│   ├── Value: #2D2D2D
│   └── Usage: Module text color
│
├── Text:1 (Secondary text)
│   └── Value: #5C5C5C
│
└── Text:2 (Muted text)
    └── Value: #7A7A7A
```

**Fonts:**

```
Fonts
├── Font:Headline
│   ├── Primary: Google Fonts → 'Inter:wght=700'
│   └── Breakpoint values:
│       ├── >980px: 700 (7pt)
│       ├── 768px: 600 (6pt)
│       └── <768px: 400 (5pt)
│
├── Font:Body
│   ├── Primary: 'Open+Sans:wght=400'
│   └── Breakpoint values:
│       ├── >980px: 400 (16pt)
│       ├── 768px: 400 (14pt)
│       └── <768px: 400 (14pt)
│
└── Font:Accent
    ├── Primary: 'Poppins:wght=600'
    └── Use for headings in specific sections
```

**Spacing:**

```
Spacing
├── Spacing:Padding
│   ├── Default: 80px (Desktop)
│   ├── Breakpoint values:
│   │   ├── >980px: 80px
│   │   ├── 768px: 60px
│   │   └── <768px: 40px
│   └── Usage: Module padding (vertical)
│
├── Spacing:Margin
│   └── Default: 0 (Desktop)
│   └── Use when module is inside container
│
└── Spacing:Gap
    └── Default: 40px (Between modules)
    └── Use for horizontal gap between columns
```

### Step 3: Apply Variables to Modules

**Method 1: Module Variable Controls**

1. Open Divi Builder
2. Add module
3. Module → Design → Variable Controls
4. Select variable from dropdown (e.g., "Primary:0")
5. Set usage (Background, Text, Border, etc.)

**Method 2: Global CSS**

1. WordPress Admin → Appearance → Customize
2. Divi → CSS → Variables
3. Paste variable definitions:
```css
:root {
  --divi-primary-0: #E40221;
  --divi-text-0: #2D2D2D;
  --divi-padding: 80px;
}
```

**Method 3: Theme Customizer**

1. WordPress Admin → Appearance → Divi
2. Theme Customizer → CSS
3. Use CSS variables with --divi-* prefix

## Using Variables in Module Design

### Color Variable Usage

```
Text Module:
├── Design → Text Color → Variable → "Text:0"
├── Design → Background Color → Variable → "Primary:0" (optional)
│
Image Module:
├── Design → Overlay Color → Variable → "Primary:0"
│
Button Module:
├── Design → Background Color → Variable → "Primary:0"
└── Design → Text Color → Variable → "Text:0"
```

### Font Variable Usage

```
Text Module:
├── Design → Font Family → Variable → "Font:Headline"
│   (for headlines)
│
├── Design → Font Family → Variable → "Font:Body"
│   (for body text)
│
└── Design → Font Size → Variable → "Font:Headline"
    (uses breakpoint values from variable)
```

### Spacing Variable Usage

```
Text Module:
├── Design → Text Padding → Variable → "Spacing:Padding"
│
Row Module:
├── Design → Spacing → Variable → "Spacing:Gap"
│
Section Module:
├── Design → Spacing → Variable → "Spacing:Padding"
```

## Breakpoint Configuration

### Setting Breakpoint Values

**News Variable Manager → Variable → Edit**

```
Example: Font size scaling

Variable: Font:Headline
├── Default: 70 (pt)
│
├── >980px:
│   ├── H-Heading: 70pt
│   └── Body: 16pt
│
├── 768px-980px:
│   ├── H-Heading: 60pt
│   └── Body: 14pt
│
└── <768px:
    ├── H-Heading: 40pt
    └── Body: 14pt
```

**Tip:** Breakpoint values are automatically applied to modules using that variable.

## Best Practices

1. **Keep variables simple**
   - Use clear names (Primary:0, Body:Primary)
   - Avoid overly complex naming

2. **Limit color palette**
   - 3-5 main colors max
   - Use variables for consistency

3. **Plan breakpoints**
   - Define values for all breakpoints
   - Test on each breakpoint

4. **Document your variables**
   - Add comments in Variable Manager
   - Keep track of why certain values are used

5. **Backup variables**
   - Export variables before major changes
   - Use Git to store variable manager snapshots

## Troubleshooting

### Variable not applying

1. Check if News Variable Manager is activated
2. Verify module is using variable from dropdown
3. Check variable has valid default value
4. Clear cache

### Variable has wrong values

1. Reopen variable in News Variable Manager
2. Check breakpoint values
3. Verify "Default" value
4. Save and refresh Divi page

### Module not responsive

1. Check if variable has breakpoint values
2. Verify module is set to use variable
3. Test on each breakpoint manually

## Example Variable Set

```yaml
Colors:
  Primary:0:
    default: "#E40221"
    values:
      desktop: "#E40221"
      tablet: "#d6021b"
      mobile: "#b90215"
  Primary:1:
    default: "hsla(0,100%,95%,1)"
    values:
      desktop: "hsla(0,100%,95%,1)"
      tablet: "hsla(0,100%,95%,1)"
      mobile: "hsla(0,100%,95%,1)"

Fonts:
  Font:Headline:
    default: "Inter:wght=700"
    values:
      desktop: "700"
      tablet: "600"
      mobile: "400"
  
  Font:Body:
    default: "Open+Sans:wght=400"
    values:
      desktop: "400"
      tablet: "400"
      mobile: "400"

Spacing:
  Spacing:Padding:
    default: "80px"
    values:
      desktop: "80px"
      tablet: "60px"
      mobile: "40px"
```

## Workflow with Variables

1. **Create variables** in News Variable Manager
2. **Set up your brand** (colors, fonts, spacing)
3. **Build page** in Divi Builder
4. **Apply variables** to modules using dropdown selectors
5. **Test breakpoints** to verify values
6. **Save to Library** for reuse
7. **Update brand** by changing variables (updates everywhere)

This approach ensures consistency across your entire site while making it easy to maintain global branding.
