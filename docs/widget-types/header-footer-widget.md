---
sidebar_position: 3
---

# Header and Footer Widget (NATIVE_FIXED_BOTTOM_AND_HEADER_ARTICLE)

The Header and Footer Widget is designed to display ads in the header and footer sections of your webpage, providing consistent ad placement while maintaining a clean user interface.

## Overview

The Header and Footer Widget is designed to:
- Display ads in header and footer sections
- Provide consistent ad placement
- Maintain website layout integrity
- Optimize for different screen sizes

## Implementation

### Basic Usage
```html
<div dg_widget_id="114" dg_widget_type="NATIVE_FIXED_BOTTOM_AND_HEADER_ARTICLE"></div>
```

### Placement in Layout
```html
<!DOCTYPE html>
<html>
<head>
  <!-- Head content -->
</head>
<body>
  <!-- Header Widget -->
  <header>
    <div dg_widget_id="114" dg_widget_type="NATIVE_FIXED_BOTTOM_AND_HEADER_ARTICLE"></div>
  </header>

  <main>
    <!-- Main content -->
  </main>

  <!-- Footer Widget -->
  <footer>
    <div dg_widget_id="114" dg_widget_type="NATIVE_FIXED_BOTTOM_AND_HEADER_ARTICLE"></div>
  </footer>
</body>
</html>
```

## Features

### 1. Layout Integration
- Seamless integration with header and footer
- Maintains website structure
- Consistent ad placement
- Responsive design

### 2. User Experience
- Non-intrusive ad placement
- Clear visual separation
- Mobile-friendly design
- Optimized for different devices

### 3. Performance
- Efficient rendering
- Minimal impact on page load
- Smart layout adaptation

## Best Practices

### Placement
1. Place in appropriate header/footer sections
2. Maintain proper spacing
3. Consider website layout
4. Ensure responsive behavior

### Configuration
1. Use appropriate widget IDs
2. Follow layout guidelines
3. Maintain consistent placement

### Layout Guidelines
1. Don't overcrowd header/footer
2. Maintain proper spacing
3. Consider mobile layout
4. Test on different devices

## Troubleshooting

### Common Issues
1. **Widget Not Displaying**
   - Check widget ID and type
   - Verify header/footer structure
   - Ensure proper placement

2. **Layout Issues**
   - Check CSS conflicts
   - Verify responsive behavior
   - Test on different devices

3. **Mobile Display Problems**
   - Test on different screen sizes
   - Check responsive design
   - Verify layout adaptation

## Examples

### Basic Implementation
```html
<!-- Header Widget -->
<header>
  <nav>
    <!-- Navigation items -->
  </nav>
  <div dg_widget_id="114" dg_widget_type="NATIVE_FIXED_BOTTOM_AND_HEADER_ARTICLE"></div>
</header>

<!-- Footer Widget -->
<footer>
  <div dg_widget_id="114" dg_widget_type="NATIVE_FIXED_BOTTOM_AND_HEADER_ARTICLE"></div>
  <div class="footer-content">
    <!-- Footer content -->
  </div>
</footer>
```

### Multiple Widgets
```html
<!-- Header with multiple widgets -->
<header>
  <div dg_widget_id="114" dg_widget_type="NATIVE_FIXED_BOTTOM_AND_HEADER_ARTICLE"></div>
  <nav>
    <!-- Navigation items -->
  </nav>
  <div dg_widget_id="115" dg_widget_type="NATIVE_FIXED_BOTTOM_AND_HEADER_ARTICLE"></div>
</header>

<!-- Footer with multiple widgets -->
<footer>
  <div dg_widget_id="114" dg_widget_type="NATIVE_FIXED_BOTTOM_AND_HEADER_ARTICLE"></div>
  <div class="footer-content">
    <!-- Footer content -->
  </div>
  <div dg_widget_id="115" dg_widget_type="NATIVE_FIXED_BOTTOM_AND_HEADER_ARTICLE"></div>
</footer>
```

## Support
For any issues with Header and Footer Widget implementation, contact our support team or refer to the [Quick Start](/docs/quick-start) guide. 