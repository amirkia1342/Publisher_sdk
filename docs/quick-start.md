---
sidebar_position: 1
---

# Quick Start

Get started with Publisher SDK in minutes. Follow these simple steps to integrate the SDK into your website.

## Installation Steps

### Step 1: Add Dauid unique Smartech id
```html
<!-- Add iframe for DIUID -->
<iframe id="diidFrame" src="https://id.lazytech.ir" style="display: none;"></iframe>
```

### Step 2: Add your widgets tags to your HTML node
```html
<!-- Add ad widgets -->
<div dg_widget_id="116" dg_widget_type="NATIVE_FLOAT"></div>
<div dg_widget_id="117" dg_widget_type="NATIVE_FLOAT"></div>
<div dg_widget_id="118" dg_widget_type="NATIVE_FIXED_MIDDLE_ARTICLE"></div>
```

### Step 3: Initialize the SDK
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

## Next Steps
- Learn about [Dauid](/docs/dauid) for user identification
- Understand the [SDK Script](/docs/sdk-script) functionality
- Explore [Widget Types](/docs/intro#ad-widget-types) for different ad placements 