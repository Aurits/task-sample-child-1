# Color System

## Overview

Our color system is designed to create a cohesive, accessible, and scalable visual language across all digital products. Colors are organized into semantic categories that communicate their intended use.

## Color Principles

1. **Accessibility First**: All color combinations meet WCAG 2.1 AA standards
2. **Semantic Meaning**: Colors convey consistent meaning across the system
3. **Systematic Scales**: Each color has a predictable scale from light to dark
4. **Context Aware**: Colors adapt to light and dark modes

## Brand Colors

### Primary Color
The primary color represents our brand and is used for primary actions and key interface elements.

```scss
$primary-50:  #EFF6FF;  // Lightest tint
$primary-100: #DBEAFE;
$primary-200: #BFDBFE;
$primary-300: #93C5FD;
$primary-400: #60A5FA;
$primary-500: #3B82F6;  // Base color
$primary-600: #2563EB;  // Hover state
$primary-700: #1D4ED8;  // Active state
$primary-800: #1E40AF;
$primary-900: #1E3A8A;  // Darkest shade
```

### Secondary Color
Used for secondary actions and supporting interface elements.

```scss
$secondary-50:  #F5F3FF;
$secondary-100: #EDE9FE;
$secondary-200: #DDD6FE;
$secondary-300: #C4B5FD;
$secondary-400: #A78BFA;
$secondary-500: #8B5CF6;  // Base color
$secondary-600: #7C3AED;
$secondary-700: #6D28D9;
$secondary-800: #5B21B6;
$secondary-900: #4C1D95;
```

## Neutral Colors

Neutral colors are used for text, backgrounds, and borders throughout the interface.

```scss
$gray-50:  #F9FAFB;  // Background
$gray-100: #F3F4F6;  // Light background
$gray-200: #E5E7EB;  // Borders
$gray-300: #D1D5DB;  // Disabled state
$gray-400: #9CA3AF;  // Placeholder text
$gray-500: #6B7280;  // Secondary text
$gray-600: #4B5563;  // Primary text
$gray-700: #374151;  // Emphasis text
$gray-800: #1F2937;  // Strong text
$gray-900: #111827;  // Headings
```

## Semantic Colors

### Success
Used for positive actions, confirmations, and success states.

```scss
$success-50:  #F0FDF4;
$success-100: #DCFCE7;
$success-200: #BBF7D0;
$success-300: #86EFAC;
$success-400: #4ADE80;
$success-500: #22C55E;  // Base
$success-600: #16A34A;
$success-700: #15803D;
$success-800: #166534;
$success-900: #14532D;
```

### Warning
Used for warnings, cautions, and attention-required states.

```scss
$warning-50:  #FFFBEB;
$warning-100: #FEF3C7;
$warning-200: #FDE68A;
$warning-300: #FCD34D;
$warning-400: #FBBF24;
$warning-500: #F59E0B;  // Base
$warning-600: #D97706;
$warning-700: #B45309;
$warning-800: #92400E;
$warning-900: #78350F;
```

### Error
Used for errors, destructive actions, and critical states.

```scss
$error-50:  #FEF2F2;
$error-100: #FEE2E2;
$error-200: #FECACA;
$error-300: #FCA5A5;
$error-400: #F87171;
$error-500: #EF4444;  // Base
$error-600: #DC2626;
$error-700: #B91C1C;
$error-800: #991B1B;
$error-900: #7F1D1D;
```

### Info
Used for informational messages and neutral states.

```scss
$info-50:  #EFF6FF;
$info-100: #DBEAFE;
$info-200: #BFDBFE;
$info-300: #93C5FD;
$info-400: #60A5FA;
$info-500: #3B82F6;  // Base
$info-600: #2563EB;
$info-700: #1D4ED8;
$info-800: #1E40AF;
$info-900: #1E3A8A;
```

## Color Usage Guidelines

### Text Colors
```scss
// Primary text (high emphasis)
color: $gray-900;

// Secondary text (medium emphasis)
color: $gray-700;

// Tertiary text (low emphasis)
color: $gray-500;

// Disabled text
color: $gray-400;

// Link text
color: $primary-600;

// Link hover
color: $primary-700;
```

### Background Colors
```scss
// Page background
background-color: $gray-50;

// Card background
background-color: white;

// Hover state
background-color: $gray-100;

// Selected state
background-color: $primary-50;

// Disabled state
background-color: $gray-200;
```

### Border Colors
```scss
// Default border
border-color: $gray-200;

// Focus border
border-color: $primary-500;

// Error border
border-color: $error-500;

// Success border
border-color: $success-500;
```

## Accessibility Considerations

### Contrast Ratios
All text colors must meet the following contrast ratios:
- **Normal text**: 4.5:1 minimum
- **Large text**: 3:1 minimum
- **UI components**: 3:1 minimum

### Color Blind Friendly
- Never use color as the only means of conveying information
- Supplement color with icons, patterns, or text
- Test designs with color blindness simulators

### Testing Tools
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- [Stark Figma Plugin](https://www.getstark.co/)
- [Colorblinding Chrome Extension](https://chrome.google.com/webstore/detail/colorblinding/)

## Dark Mode

### Dark Mode Palette
```scss
// Backgrounds
$dark-bg-primary: #0F172A;
$dark-bg-secondary: #1E293B;
$dark-bg-tertiary: #334155;

// Text
$dark-text-primary: #F8FAFC;
$dark-text-secondary: #E2E8F0;
$dark-text-tertiary: #CBD5E1;

// Borders
$dark-border: #334155;
$dark-border-hover: #475569;
```

### Color Mapping
```scss
// Light mode ’ Dark mode
$gray-50  ’ $dark-bg-primary
$gray-100 ’ $dark-bg-secondary
$gray-200 ’ $dark-bg-tertiary
$gray-900 ’ $dark-text-primary
$gray-700 ’ $dark-text-secondary
$gray-500 ’ $dark-text-tertiary
```

## Implementation

### CSS Variables
```css
:root {
  /* Primary */
  --color-primary-50: #EFF6FF;
  --color-primary-100: #DBEAFE;
  --color-primary-200: #BFDBFE;
  --color-primary-300: #93C5FD;
  --color-primary-400: #60A5FA;
  --color-primary-500: #3B82F6;
  --color-primary-600: #2563EB;
  --color-primary-700: #1D4ED8;
  --color-primary-800: #1E40AF;
  --color-primary-900: #1E3A8A;
  
  /* Semantic */
  --color-success: #22C55E;
  --color-warning: #F59E0B;
  --color-error: #EF4444;
  --color-info: #3B82F6;
}

[data-theme="dark"] {
  /* Dark mode overrides */
  --color-bg-primary: #0F172A;
  --color-text-primary: #F8FAFC;
}
```

### Tailwind Config
```js
module.exports = {
  theme: {
    colors: {
      primary: {
        50: '#EFF6FF',
        100: '#DBEAFE',
        // ... rest of scale
      },
      gray: {
        50: '#F9FAFB',
        100: '#F3F4F6',
        // ... rest of scale
      },
      // ... other colors
    }
  }
}
```

## Color Combinations

### Recommended Pairings
```scss
// Primary button
background: $primary-600;
color: white;
&:hover {
  background: $primary-700;
}

// Secondary button
background: $gray-200;
color: $gray-700;
&:hover {
  background: $gray-300;
}

// Success message
background: $success-50;
color: $success-800;
border: 1px solid $success-200;

// Error message
background: $error-50;
color: $error-800;
border: 1px solid $error-200;
```

## Migration Guide

When updating from previous color system:
1. Map old color variables to new semantic colors
2. Update component styles to use new variables
3. Test all color combinations for accessibility
4. Update documentation and design files

---

**Version**: 2.0  
**Last Updated**: January 2025  
**Contact**: design-system@example.com