# Order Summary Card Component

## Overview

This is a static frontend component project that implements an order summary card interface. It's a fully completed responsive UI component that displays subscription plan information with interactive elements. The project is built using vanilla HTML and CSS with no backend, database, or JavaScript functionality. The component successfully matches the design specifications with proper hover states, focus indicators for accessibility, and responsive design from mobile to desktop.

## Recent Changes

**September 30, 2025**
- ✅ Completed full HTML structure with semantic markup
- ✅ Implemented responsive CSS with mobile-first approach
- ✅ Added hover states for all interactive elements (buttons and links)
- ✅ Implemented focus-visible styles for keyboard accessibility
- ✅ Organized all image assets in /images directory
- ✅ Set up Python HTTP server workflow on port 5000
- ✅ Tested and verified responsive design works correctly across viewports

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture

**Component-Based HTML Structure**
- The project uses semantic HTML5 with a single-page component architecture
- Main container wraps an `<article>` element representing the order card
- Component is structured with clear sections: header (hero image), body (content), and interactive elements
- Uses semantic tags (`<main>`, `<article>`, `<h1>`, `<h2>`) for better accessibility and SEO

**CSS Design System**
- Custom properties (CSS variables) define the design system's color palette
- Two sets of color variables: one following the style guide (HSL values) and custom colors in HEX format
- Mobile-first responsive approach with background image swapping for different screen sizes
- Maximum card width constraint (450px) with centered flexbox layout for optimal viewing on all devices

**Typography System**
- Google Fonts integration for "Red Hat Display" with multiple font weights (500, 700, 900)
- Font stack includes fallbacks to system fonts for better performance
- Base font size of 16px for body copy as per accessibility guidelines

**Layout Strategy**
- Flexbox-based centering for both viewport and internal card elements
- Full viewport height layout with vertical and horizontal centering
- Card uses border-radius for rounded corners with hidden overflow for the hero image
- Responsive padding system to maintain proper spacing on mobile devices

**Visual Design Decisions**
- Background pattern image positioned at top center, non-repeating
- Card has white background with shadow effect (implied by the structure)
- Border-radius of 20px for modern, friendly appearance
- Separate background images for mobile and desktop views

### Styling Architecture

**CSS Reset and Box Model**
- Universal reset removes default browser margins and paddings
- Box-sizing set to border-box for predictable sizing calculations

**Component Isolation**
- Single CSS file approach suitable for small-scale component
- Class-based naming convention (.order-card, .card-header, .card-body, etc.)
- Modular class structure allows for easy maintenance and modifications

**Interactive Elements**
- Primary button (.btn-primary) for main call-to-action with hover and focus states
- Secondary link (.btn-cancel) for cancellation option with hover and focus states
- Change link (.plan-change) for plan modification with hover and focus states
- All interactive elements include smooth transitions and accessibility-focused :focus-visible indicators

### Responsive Design Strategy

**Breakpoint Approach**
- Mobile-first design starting at 375px design width
- Desktop design targets 1440px width
- Background image switches between mobile and desktop versions
- Content should be responsive across full range (320px to large screens)

**Constraints and Considerations**
- Maximum card width prevents excessive stretching on large screens
- Container uses percentage-based width (100%) up to max-width
- Padding on body element ensures content doesn't touch viewport edges on small screens

## External Dependencies

### Font Services
- **Google Fonts**: Hosts the "Red Hat Display" font family
  - Preconnect links optimize font loading performance
  - Display=swap parameter prevents invisible text during font load
  - Weights: 500 (medium), 700 (bold), 900 (black)

### Assets and Images
- **Local Image Assets**: All images stored in `/images` directory
  - `favicon-32x32.png`: Browser tab icon
  - `illustration-hero.png`: Hero banner image showing person with headphones
  - `icon-music.png`: Music icon for plan details section
  - `pattern-background-mobile.png`: Mobile background pattern
  - `pattern-background-desktop.png`: Desktop background pattern (switches at 768px breakpoint)

### Design Resources
- **Frontend Mentor**: Original challenge provider
  - Design specifications in `/design` folder (JPG format)
  - Style guide document provides color palette and typography specifications
  - No API or external data sources required

### Browser Compatibility
- Modern browser features used: CSS custom properties, flexbox
- Meta viewport tag ensures proper mobile rendering
- No polyfills or transpilation required for target audience
- System font fallbacks ensure text renders even if Google Fonts fails