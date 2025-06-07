# Overview
This responsive e-commerce website provides a seamless online shopping experience for merchandise buyers. The design focuses on clear navigation, trustworthy dealer connections, and straightforward shopping processes.

## Color System

### Palette & Rationale
- **Primary**: `#E74C3C` (Vibrant Red)  
  Represents energy, urgency, and call-to-action elements
- **Secondary**: `#2C3E50` (Deep Navy)  
  Conveys trust, professionalism, and stability
- **Accent**: `#F39C12` (Warm Orange)  
  Highlights important features and interactive elements
- **Background**: `#F9F9F9` (Off-White)  
  Clean canvas for content with reduced eye strain
- **Text**: `#333333` (Charcoal)  
  Primary text color for optimal readability
- **Light Text**: `#FFFFFF` (Pure White)  
  For text on colored backgrounds

**Rationale**: The red-orange palette creates a sense of urgency for shopping actions, while navy conveys reliability for dealer relationships. The neutral background ensures content remains the focus.

## Breakpoint Logic

The design follows a mobile-first approach with these key breakpoints:

```css
/* Base: Mobile (1 column) */
.container {
  width: 100%;
  padding: 0 15px;
}

/* Small devices (≥576px) */
@media (min-width: 576px) {
  .services-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

/* Medium devices (≥768px) */
@media (min-width: 768px) {
  .hero-content {
    flex-direction: row;
  }
  .testimonials {
    grid-template-columns: repeat(2, 1fr);
  }
}

/* Large devices (≥992px) */
@media (min-width: 992px) {
  .category-grid {
    grid-template-columns: repeat(3, 1fr);
  }
  .services-grid {
    grid-template-columns: repeat(4, 1fr);
  }
}

/* Extra large (≥1200px) */
@media (min-width: 1200px) {
  .container {
    max-width: 1140px;
  }
}
```

Key responsive behaviors:
- **SM (576px+)**:
  - Services grid becomes 2 columns
  - FAQ items switch to side-by-side layout
- **MD (768px+)**:
  - Hero section switches to horizontal layout
  - Testimonials become 2 columns
- **LG (992px+)**:
  - Category grid becomes 3 columns
  - Services grid becomes 4 columns
- **XL (1200px+)**:
  - Max-width container applied

## Creative Divergences

Beyond the mockup, these enhancements were implemented:

1. **Interactive Elements**:
   - Animated hover states for category cards
   - Interactive FAQ accordions with smooth transitions
   - Form validation with visual feedback

2. **Navigation Improvements**:
   - Consolidated navigation items into dropdown menus
   - Added sticky header with active state indicators
   - Included breadcrumb navigation for deeper pages

3. **Enhanced Visual Hierarchy**:
   - Created consistent card design system
   - Added subtle shadows and hover effects
   - Implemented custom icon set for services

4. **Performance Features**:
   - Lazy-loaded images for faster loading
   - Optimized image compression
   - CSS minification and concatenation

5. **Accessibility**:
   - ARIA labels for interactive elements
   - Sufficient color contrast ratios
   - Keyboard navigation support

6. **Additional Sections**:
   - Newsletter signup component in footer
   - Social proof badges for trusted dealers
   - Progress indicators for shopping steps
