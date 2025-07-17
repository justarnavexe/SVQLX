# SVQLX Unified Theme System 2025

## Overview

This project now uses a unified theme system that provides consistency across all components while maintaining a modern, professional appearance. The theme is built using CSS custom properties (variables) for easy customization and maintenance.

## Theme Structure

### Core Files
- `theme.css` - Main theme file containing all variables and base styles
- All HTML files now import this theme via `<link rel="stylesheet" href="theme.css">`

### Color Scheme

The theme uses a sophisticated dark color palette with blue and purple gradients:

**Primary Colors:**
- Background: Gradient from slate-900 to slate-700
- Secondary Background: Semi-transparent slate-900
- Tertiary Background: Semi-transparent slate-800

**Accent Colors:**
- Primary: Blue (#3b82f6)
- Secondary: Purple (#8b5cf6)
- Success: Green (#10b981)
- Warning: Yellow (#f59e0b)
- Error: Red (#ef4444)

**Text Colors:**
- Primary: Light gray (#f8fafc)
- Secondary: Medium gray (#cbd5e1)
- Muted: Darker gray (#94a3b8)

### Design System

#### Glass Morphism
The theme extensively uses glass morphism effects:
- Subtle transparency with backdrop blur
- Soft borders and shadows
- Layered depth perception

#### Gradients
Multiple gradient variations for different use cases:
- Primary: Blue to purple
- Secondary: Cyan to blue
- Accent: Green to cyan
- Warm: Yellow to red

#### Spacing System
Consistent spacing using CSS custom properties:
- `--space-xs`: 0.5rem (8px)
- `--space-sm`: 1rem (16px)
- `--space-md`: 1.5rem (24px)
- `--space-lg`: 2rem (32px)
- `--space-xl`: 3rem (48px)

#### Border Radius
Consistent border radius values:
- `--radius-sm`: 8px
- `--radius-md`: 12px
- `--radius-lg`: 16px
- `--radius-xl`: 24px
- `--radius-full`: 50%

#### Typography
- Font Family: Inter, Segoe UI, system fonts
- Font Weights: 400 (normal), 500 (medium), 600 (semibold), 700 (bold)
- Smooth font rendering enabled

#### Shadows
Multiple shadow variations for different elevations:
- `--shadow-sm`: Subtle shadow for small elements
- `--shadow-md`: Medium shadow for cards
- `--shadow-lg`: Large shadow for prominent elements
- `--shadow-xl`: Extra large shadow for modals/overlays
- `--shadow-glow`: Special glow effect for interactive elements

## Component Classes

### Containers
- `.container`: Main content container with max-width
- `.container-sm`: Smaller max-width variant
- `.container-lg`: Larger max-width variant

### Glass Components
- `.glass`: Basic glass morphism effect
- `.glass-card`: Enhanced glass card with padding and shadows

### App Components
- `.app-container`: Main app wrapper with centering
- `.app-main`: Standard app content container

### Headers
- `.header`: Standard header styling
- `.header-title`: Header title with gradient text

### Buttons
- `.btn`: Base button class
- `.btn-primary`: Primary action button with gradient
- `.btn-secondary`: Secondary button with glass effect
- `.btn-icon`: Icon-only button

### Input Elements
- `.input`: Standard input field styling

### Cards
- `.card`: Basic card component
- `.card-header`: Card header section
- `.card-title`: Card title styling
- `.card-subtitle`: Card subtitle styling

### Layout Utilities
- `.grid`: CSS Grid container
- `.grid-2`, `.grid-3`, `.grid-4`: Responsive grid columns
- `.flex`, `.flex-col`: Flexbox utilities
- `.items-center`, `.justify-center`, `.justify-between`: Alignment utilities
- `.gap-sm`, `.gap-md`, `.gap-lg`: Gap utilities

### Text Utilities
- `.text-center`: Center text alignment
- `.text-primary`, `.text-secondary`, `.text-muted`: Text color utilities
- `.text-accent`: Gradient text effect

### Status Colors
- `.status-success`, `.status-warning`, `.status-error`: Status text colors
- `.bg-success`, `.bg-warning`, `.bg-error`: Status background colors

### Animations
- `.animate-slideUp`: Slide up animation
- `.animate-fadeIn`: Fade in animation
- `.animate-float`: Floating animation

## Responsive Design

The theme includes responsive breakpoints:
- Mobile: ≤ 480px
- Tablet: ≤ 768px
- Desktop: > 768px

## Customization

### Changing Colors
To customize colors, modify the CSS custom properties in the `:root` selector of `theme.css`:

```css
:root {
    --accent-primary: #your-color;
    --gradient-primary: linear-gradient(135deg, #color1, #color2);
}
```

### Adding New Components
Follow the established patterns:
1. Use CSS custom properties for consistency
2. Apply glass morphism effects where appropriate
3. Include hover states and transitions
4. Ensure responsive behavior

### Light Mode Support
The theme includes basic light mode support via CSS media queries. Components can opt into light mode by adding the `.light-mode` class.

## Browser Support

The theme uses modern CSS features:
- CSS Custom Properties
- CSS Grid
- Flexbox
- Backdrop Filter
- CSS Gradients

Supported browsers:
- Chrome 49+
- Firefox 31+
- Safari 9.1+
- Edge 16+

## Performance Considerations

- CSS variables enable efficient theme switching
- Backdrop filters are used sparingly to avoid performance issues
- Animations use hardware acceleration where possible
- Font loading is optimized with system font fallbacks

## Migration from Old Themes

All HTML files have been updated to:
1. Import the unified theme CSS file
2. Remove redundant CSS reset code
3. Use theme variables instead of hardcoded values
4. Maintain original functionality while improving consistency

## Best Practices

1. **Always use CSS custom properties** for colors, spacing, and other theme values
2. **Maintain semantic class names** that describe purpose, not appearance
3. **Test responsive behavior** on different screen sizes
4. **Use the established spacing system** instead of arbitrary values
5. **Follow the glass morphism pattern** for new components
6. **Include proper hover and focus states** for interactive elements

## Future Enhancements

Potential improvements:
- Theme switching functionality (dark/light toggle)
- Additional color scheme variants
- More animation utilities
- Enhanced accessibility features
- CSS-in-JS integration options