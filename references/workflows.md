# Divi Workflows

Step-by-step workflows for common Divi website creation tasks.

## Workflow 1: Create Page from HTML Mockup

### Step 1: Analyze HTML Structure

1. Open HTML file
2. Identify sections (header, hero, features, footer, etc.)
3. Note CSS classes for styling hints
4. Extract images and assets
5. Document color scheme and typography

### Step 2: Plan Divi Structure

Create a mapping document:

```
HTML Section → Divi Section Type
├── Container → Row settings (max-width, padding)
├── Row → Divi Row
├── Columns → Divi Columns
└── Elements → Divi Modules
```

### Step 3: Create WordPress Page

1. WordPress Admin → Pages → Add New
2. Enter page title
3. Click "Use Divi Builder"
4. Select "Build from Scratch" or appropriate layout

### Step 4: Build Sections (Top to Bottom)

For each HTML section:

1. **Add Section** (Regular/Fullwidth/Specialty)
2. **Configure Section**
   - Background (color/image/gradient)
   - Spacing (padding/margin)
   - Advanced effects (parallax, animations)
3. **Add Rows** matching HTML structure
4. **Add Columns** with appropriate widths
5. **Add Modules** corresponding to HTML elements

### Step 5: Configure Modules

For each module:

1. **Content Tab**: Add text, images, URLs
2. **Design Tab**: 
   - Typography (font, size, color)
   - Spacing (margin, padding)
   - Border
   - Background
   - Animation
3. **Advanced Tab**: 
   - CSS ID/Class (if needed)
   - Custom CSS
   - Visibility

### Step 6: Responsive Adjustments

1. Switch to **Tablet** view
2. Adjust font sizes, spacing, column order
3. Switch to **Mobile** view
4. Hide non-essential elements if needed
5. Check all breakpoints

### Step 7: Final Review

1. Preview page on desktop
2. Test responsive views
3. Check all links work
4. Verify forms submit correctly
5. Save draft or publish

---

## Workflow 2: Create Page from Design Description

### Step 1: Understand Requirements

Ask clarifying questions:

- What's the page purpose? (landing, about, contact, etc.)
- What's the target audience?
- Any specific colors or branding?
- What content needs to be included?
- Any special functionality? (forms, sliders, etc.)

### Step 2: Choose Layout Pattern

Refer to [layout-patterns.md](layout-patterns.md):

- Landing page → Hero + Features + CTA + Footer
- About page → Hero + Story + Team + Values
- Contact page → Hero + Form + Map + Info
- Portfolio → Hero + Filterable Grid

### Step 3: Plan Sections

Sketch the page structure:

```
1. Hero Section (Fullwidth, headline, CTA)
2. Features Section (3 columns, icons)
3. About Section (2 columns, image + text)
4. Testimonials Section (slider)
5. CTA Section (fullwidth color)
6. Footer
```

### Step 4-7: Same as Workflow 1

---

## Workflow 3: Recreate Existing Website

### Step 1: Analyze Target Site

1. Screenshot full page
2. Identify all sections
3. Note interactive elements
4. Document colors (use browser inspector)
5. Identify fonts
6. Save reference images

### Step 2: Gather Assets

1. Logo (SVG preferred)
2. Product images
3. Team photos
4. Icons
5. Any custom graphics

### Step 3: Map to Divi

Section by section:

```
Target Site Section → Divi Implementation
Header → Theme Builder Header
Hero → Fullwidth Section + Slider
Features → 3-column Row + Blurbs
etc.
```

### Step 4: Build Iteratively

1. Build one section at a time
2. Compare with reference
3. Adjust until matching
4. Move to next section

### Step 5: Fine-tuning

1. Match exact colors (hex codes)
2. Match exact spacing (pixel values)
3. Replicate hover effects
4. Match animations if possible

---

## Workflow 4: Create Landing Page

### Step 1: Define Conversion Goal

What action should visitors take?

- Sign up for email list
- Purchase product
- Request demo
- Download resource

### Step 2: Plan Content Flow

```
1. Hook (Hero headline)
2. Problem/Agitation
3. Solution (Features/Benefits)
4. Proof (Testimonials/Stats)
5. CTA
6. FAQ (address objections)
7. Final CTA
```

### Step 3: Build Sections

**Hero:**
- Compelling headline
- Subheadline
- Primary CTA button
- Supporting image/video

**Features:**
- 3-6 key benefits
- Icons + short descriptions
- Visual hierarchy

**Social Proof:**
- Testimonials
- Logos of clients/press
- Statistics

**FAQ:**
- Address common objections
- Accordion or toggle modules

**CTA Sections:**
- Repeat CTA throughout
- Urgency elements (countdown, limited spots)

### Step 4: Optimize for Conversion

1. Clear, prominent CTAs
2. Contrasting button colors
3. Minimal navigation distractions
4. Fast loading
5. Mobile-optimized

---

## Workflow 5: Import/Export Layouts

### Export Layout (for reuse)

1. Open page in Divi Builder
2. Click "···" (three dots) in purple bar
3. Select "Save to Library"
4. Name the layout
5. Choose category (optional)
6. Save

### Import Layout

1. Create new page
2. Open Divi Builder
3. Click "+" (Add From Library)
4. Switch to "Saved Layouts"
5. Find and select layout
6. Click "Load"

### Export for Another Site

1. Divi → Divi Library
2. Find saved layout
3. Export as JSON
4. Import on target site: Divi → Import & Export

---

## Workflow 6: Build with Theme Builder

### Step 1: Plan Templates

What custom templates do you need?

- Global Header (site-wide)
- Global Footer (site-wide)
- Single Post template
- Category archive
- Custom 404 page
- Search results

### Step 2: Create Header Template

1. Divi → Theme Builder
2. Add Global Header
3. Build with Theme Builder
4. Common elements:
   - Logo
   - Navigation menu
   - CTA button
   - Social icons
5. Set mobile menu style

### Step 3: Create Footer Template

1. Add Global Footer
2. Build columns:
   - Logo + About
   - Quick Links
   - Contact Info
   - Newsletter
3. Add copyright bar

### Step 4: Create Post Template

1. Add template for "All Posts"
2. Include:
   - Featured image
   - Post title
   - Post content module
   - Author box
   - Related posts
   - Comments

### Step 5: Create Archive Template

1. Add template for "All Category Pages"
2. Include:
   - Archive title
   - Blog module (posts from current category)

### Step 6: Assign Templates

Set display rules:
- Specific pages
- Post types
- Categories
- Tags
- etc.

---

## Best Practices

### Naming Conventions

- Sections: Descriptive ("Hero Section", "Features Section")
- Rows: Purpose-based ("2-Column Row", "Centered Row")
- Modules: Content-based ("Welcome Text", "CTA Button")

### Organization

- Group related sections
- Use consistent spacing
- Limit colors to brand palette
- Reuse global modules when possible

### Performance

- Optimize images before upload
- Use appropriate image sizes
- Enable caching
- Minimize heavy animations

### Accessibility

- Add alt text to images
- Ensure sufficient color contrast
- Use semantic headings (H1, H2, H3)
- Make buttons large enough to click
- Test with keyboard navigation

### Maintenance

- Save reusable sections to Library
- Document custom CSS
- Keep backups of layouts
- Update Divi regularly
