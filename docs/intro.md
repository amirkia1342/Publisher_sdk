---
sidebar_position: 1
---

# Publisher SDK

## Introduction
Publisher SDK is a powerful tool for displaying intelligent advertisements and recommended content on websites. This SDK allows you to easily implement various advertising widgets on your website.

### Key Features
- 🎯 Smart ad display based on user behavior
- 📱 Support for various ad widgets (floating, middle article, header and footer)
- 🔄 Automatic optimization for different devices (mobile, tablet, desktop)
- 📊 Advanced reporting system
- 🚀 Fast and optimized performance
- 🔒 High security using DIUID

## Installation and Setup

###  Step 1: Add Dauid unique Smartech id:
```html
<!-- Add iframe for DIUID -->
<iframe id="diidFrame" src="https://id.lazytech.ir" style="display: none;"></iframe>
```
### Step 2: Add your widgets tags to your HTML node:
```html

<!-- Add ad widgets -->
<div dg_widget_id="116" dg_widget_type="NATIVE_FLOAT"></div>
<div dg_widget_id="117" dg_widget_type="NATIVE_FLOAT"></div>
<div dg_widget_id="118" dg_widget_type="NATIVE_FIXED_MIDDLE_ARTICLE"></div>
```

### Step 3: Usage SDK in Projects
```javascript
// In index.html
<script type="text/javascript">
    (function(w, d, s, src, fnName) {
      w[fnName] = w[fnName] || function() {
        (w[fnName].q = w[fnName].q || []).push(arguments);
      };
      var script = d.createElement(s);
      script.async = true;
      script.src = src;
      script.onload = function() {
        function initPublisher(retry = 0) {
          if (retry > 50) {
            return;
          }
          if (!w.Publisher || !w.Publisher.getInstance || !document.querySelector('[dg_widget_id]')) {
            setTimeout(() => initPublisher(retry + 1), 100);
            return;
          }
          w.Publisher.getInstance().then(function(publisher) {
          }).catch(function(err) {
            setTimeout(() => initPublisher(retry + 1), 100);
          });
        }
        initPublisher();
      };
      var firstScript = d.getElementsByTagName(s)[0];
      firstScript.parentNode.insertBefore(script, firstScript);
    })(window, document, 'script', 'https://publisher-sdk.lazytech.ir/publisher.js', 'Publisher');
  </script>
```

## Ad Widget Types

### 1. Floating Widget (NATIVE_FLOAT)
```html
<div dg_widget_id="116" dg_widget_type="NATIVE_FLOAT"></div>
```
- Displays ads floating on the page
- Suitable for increasing click-through rates
- Compatible with all devices

### 2. Middle Article Widget (NATIVE_FIXED_MIDDLE_ARTICLE)
```html
<div dg_widget_id="118" dg_widget_type="NATIVE_FIXED_MIDDLE_ARTICLE"></div>
```
- Displays ads within article content
- Design consistent with page content
- Optimized for readability

### 3. Header and Footer Widget (NATIVE_FIXED_BOTTOM_AND_HEADER_ARTICLE)
```html
<div dg_widget_id="114" dg_widget_type="NATIVE_FIXED_BOTTOM_AND_HEADER_ARTICLE"></div>
```
- Displays ads in header and footer
- Capable of showing multiple ads
- Responsive design

## Error Handling and Troubleshooting

### Common Errors
1. **Missing Widget Elements**
   - Ensure DOM is fully loaded
   - Verify widget IDs
   - Check HTML structure

2. **DIUID Errors**
   - Ensure DIUID iframe exists
   - Check access to id.lazytech.ir domain
   - Verify CORS settings

### Logging and Reporting
- Use `console.log` for status checking
- Check Network tab in DevTools
- Use built-in SDK reporting system

## Best Practices

### Performance Optimization
1. Load script with `async` or `defer`
2. Place widgets in appropriate positions
3. Use lazy loading for non-essential widgets

### Security
1. Use HTTPS
2. Validate input data
3. Protect against XSS

## Support and Contribution
- Report bugs in Issues section
- Submit Pull Requests for code improvements
- Contribute to development and documentation

## License
This project is licensed under the MIT License.
