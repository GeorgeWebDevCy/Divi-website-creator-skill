# HTML to Divi Mapping

Guide for converting HTML structures into Divi layouts.

## Common HTML to Divi Conversions

### Header / Navigation

**HTML:**
```html
<header>
  <nav>
    <ul>
      <li><a href="/">Home</a></li>
      <li><a href="/about">About</a></li>
      <li><a href="/contact">Contact</a></li>
    </ul>
  </nav>
</header>
```

**Divi:**
- Use **Menu Module** in Theme Builder Header template
- Or create custom navigation using Button modules

### Hero Section

**HTML:**
```html
<section class="hero">
  <div class="container">
    <h1>Main Headline</h1>
    <p>Subheadline text</p>
    <a href="#" class="btn">Get Started</a>
  </div>
</section>
```

**Divi:**
```
Section (Fullwidth)
└── Row (Centered)
    └── Column (1 column)
        ├── Text Module (H1 - Headline)
        ├── Text Module (P - Subheadline)
        └── Button Module (CTA)
```

### Two-Column Layout

**HTML:**
```html
<section>
  <div class="row">
    <div class="col-6">
      <img src="image.jpg" alt="Description">
    </div>
    <div class="col-6">
      <h2>Section Title</h2>
      <p>Description text...</p>
      <a href="#" class="btn">Learn More</a>
    </div>
  </div>
</section>
```

**Divi:**
```
Section
└── Row (2 columns - 1/2 + 1/2)
    ├── Column 1
    │   └── Image Module
    └── Column 2
        ├── Text Module (H2 - Title)
        ├── Text Module (P - Description)
        └── Button Module
```

### Feature Grid (3 Columns)

**HTML:**
```html
<section>
  <div class="row">
    <div class="col-4">
      <img src="icon1.svg" alt="">
      <h3>Feature 1</h3>
      <p>Description</p>
    </div>
    <div class="col-4">
      <img src="icon2.svg" alt="">
      <h3>Feature 2</h3>
      <p>Description</p>
    </div>
    <div class="col-4">
      <img src="icon3.svg" alt="">
      <h3>Feature 3</h3>
      <p>Description</p>
    </div>
  </div>
</section>
```

**Divi:**
```
Section
└── Row (3 columns - 1/3 + 1/3 + 1/3)
    ├── Column 1
    │   └── Blurb Module (Icon + Title + Text)
    ├── Column 2
    │   └── Blurb Module
    └── Column 3
        └── Blurb Module
```

### Call-to-Action Section

**HTML:**
```html
<section class="cta">
  <div class="container">
    <h2>Ready to Get Started?</h2>
    <p>Join thousands of satisfied customers.</p>
    <a href="/signup" class="btn-primary">Sign Up Now</a>
  </div>
</section>
```

**Divi:**
```
Section (Specialty - Add background color/image)
└── Row (Centered, narrow width)
    └── Column (1 column)
        └── Call To Action Module
            ├── Title: "Ready to Get Started?"
            ├── Body: "Join thousands..."
            └── Button: "Sign Up Now"
```

### Testimonials

**HTML:**
```html
<section>
  <div class="testimonial">
    <blockquote>"Amazing service!" </blockquote>
    <cite>John Doe, CEO</cite>
    <img src="john.jpg" alt="John Doe">
  </div>
</section>
```

**Divi:**
```
Section
└── Row
    └── Column
        └── Testimonial Module
            ├── Quote: "Amazing service!"
            ├── Author: "John Doe"
            ├── Job Title: "CEO"
            └── Image: john.jpg
```

### Contact Form

**HTML:**
```html
<form>
  <input type="text" name="name" placeholder="Name">
  <input type="email" name="email" placeholder="Email">
  <textarea name="message" placeholder="Message"></textarea>
  <button type="submit">Send</button>
</form>
```

**Divi:**
```
Section
└── Row
    └── Column
        └── Contact Form Module
            ├── Fields: Name, Email, Message
            └── Submit Button: "Send"
```

## CSS to Divi Settings Mapping

### Colors

| CSS | Divi Setting |
|-----|--------------|
| `background-color` | Section/Row/Module → Background |
| `color` | Module → Text Color |
| `border-color` | Module → Border → Color |

### Typography

| CSS | Divi Setting |
|-----|--------------|
| `font-family` | Module → Text → Font |
| `font-size` | Module → Text → Size |
| `font-weight` | Module → Text → Weight |
| `line-height` | Module → Text → Line Height |
| `text-align` | Module → Text → Alignment |

### Spacing

| CSS | Divi Setting |
|-----|--------------|
| `margin` | Module → Spacing → Margin |
| `padding` | Module → Spacing → Padding |
| Section padding | Section → Spacing → Padding |

### Layout

| CSS | Divi Setting |
|-----|--------------|
| `display: flex` | Row settings, Column alignment |
| `justify-content` | Row → Column Alignment |
| `align-items` | Module → Vertical Alignment |

## Responsive Mapping

### Media Queries to Divi Breakpoints

```css
/* Desktop */
@media (min-width: 981px) { }
/* → Divi Desktop tab */

/* Tablet */
@media (max-width: 980px) { }
/* → Divi Tablet tab */

/* Mobile */
@media (max-width: 767px) { }
/* → Divi Mobile tab */
```

### Common Responsive Patterns

**Stack columns on mobile:**
- Divi: Row → Column Settings → Responsive → Enable "Stack on Mobile"

**Hide elements on mobile:**
- Divi: Module → Advanced → Visibility → Disable on Phone/Tablet

**Different font sizes per device:**
- Divi: Module → Text → Size → Desktop/Tablet/Phone values
