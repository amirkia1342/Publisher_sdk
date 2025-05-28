---
sidebar_position: 3
---

# SDK Script

The Publisher SDK script is the core component that enables intelligent ad delivery and content recommendation on your website.

## Overview

The SDK script provides:
- Widget initialization and management
- Ad delivery optimization
- User behavior tracking
- Performance monitoring
- Error handling and reporting

## Implementation

### Basic Integration
```javascript
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

## Features

### 1. Automatic Initialization
- Self-initializing script
- Retry mechanism for reliable loading
- Automatic widget detection

### 2. Performance Optimization
- Async loading
- Minimal impact on page load
- Efficient resource management

### 3. Error Handling
- Automatic retry on failure
- Detailed error reporting
- Graceful degradation

## Best Practices

### Loading
1. Place the script in the `<head>` section
2. Use async loading
3. Ensure Dauid iframe is loaded first

### Configuration
1. Don't modify the script source URL
2. Keep the script parameters unchanged
3. Maintain proper initialization order

### Performance
1. Minimize DOM modifications
2. Use appropriate widget types
3. Monitor script performance

## Troubleshooting

### Common Issues
1. **Script Not Loading**
   - Check network connectivity
   - Verify script URL accessibility
   - Check browser console for errors

2. **Widgets Not Displaying**
   - Verify widget IDs
   - Check initialization status
   - Ensure proper DOM structure

3. **Performance Issues**
   - Monitor script load time
   - Check widget rendering
   - Review error logs

## Support
For technical support or questions about the SDK script, contact our support team or refer to the [Quick Start](/docs/quick-start) guide. 