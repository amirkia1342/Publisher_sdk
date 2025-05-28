---
sidebar_position: 1
---

# Floating Widget (NATIVE_FLOAT)

The Floating Widget is a dynamic ad display component that appears as a floating element on your webpage, providing maximum visibility while maintaining a good user experience.

## Overview

The Floating Widget is designed to:
- Display ads in a floating position on the page
- Automatically adjust position based on user interaction
- Provide high visibility without disrupting content
- Optimize for different screen sizes

## Implementation

### Basic Usage
```html
<div dg_widget_id="116" dg_widget_type="NATIVE_FLOAT"></div>
```

### Multiple Floating Widgets
```html
<!-- You can add multiple floating widgets with different IDs -->
<div dg_widget_id="116" dg_widget_type="NATIVE_FLOAT"></div>
<div dg_widget_id="117" dg_widget_type="NATIVE_FLOAT"></div>
```

## Features

### 1. Smart Positioning
- Automatically positions itself for optimal visibility
- Avoids overlapping with important content
- Responsive to user scrolling and interaction

### 2. User Experience
- Non-intrusive design
- Smooth animations
- Easy to close or minimize
- Mobile-friendly

### 3. Performance
- Lightweight implementation
- Minimal impact on page load
- Efficient resource usage

## Best Practices

### Placement
1. Avoid placing multiple floating widgets too close to each other
2. Consider user's reading flow
3. Ensure widgets don't block important content

### Configuration
1. Use unique widget IDs for each floating widget
2. Maintain consistent widget types
3. Follow the recommended implementation pattern

### User Experience
1. Don't overload the page with too many floating widgets
2. Ensure widgets are easily dismissible
3. Test on different devices and screen sizes

## Troubleshooting

### Common Issues
1. **Widget Not Floating**
   - Check widget ID and type
   - Verify SDK initialization
   - Ensure proper DOM structure

2. **Positioning Problems**
   - Check for CSS conflicts
   - Verify viewport settings
   - Test on different screen sizes

3. **Performance Issues**
   - Monitor widget load time
   - Check for multiple instances
   - Review resource usage

## Examples

### Basic Implementation
```html
<!-- Single floating widget -->
<div dg_widget_id="116" dg_widget_type="NATIVE_FLOAT"></div>
```

### Multiple Widgets
```html
<!-- Multiple floating widgets with different positions -->
<div dg_widget_id="116" dg_widget_type="NATIVE_FLOAT"></div>
<div dg_widget_id="117" dg_widget_type="NATIVE_FLOAT"></div>
<div dg_widget_id="118" dg_widget_type="NATIVE_FLOAT"></div>
```

## Support
For any issues with Floating Widget implementation, contact our support team or refer to the [Quick Start](/docs/quick-start) guide. 