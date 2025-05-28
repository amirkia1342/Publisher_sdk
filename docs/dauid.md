---
sidebar_position: 2
---

# Dauid

Dauid (Device Unique ID) is a unique identifier system used by Publisher SDK to track and optimize ad delivery for each user's device.

## What is Dauid?

Dauid is a unique identifier that helps in:
- Tracking user behavior across sessions
- Optimizing ad delivery based on user preferences
- Maintaining user privacy while providing personalized content
- Ensuring accurate analytics and reporting

## Implementation

### Basic Setup
```html
<!-- Add iframe for DIUID -->
<iframe id="diidFrame" src="https://id.lazytech.ir" style="display: none;"></iframe>
```

### Best Practices
1. Place the iframe in the `<head>` section of your HTML
2. Ensure the iframe is loaded before the Publisher SDK script
3. Keep the iframe hidden (display: none)
4. Don't modify the iframe's ID or source URL

## Security

Dauid implementation follows strict security guidelines:
- HTTPS-only communication
- No personal data collection
- Encrypted data transmission
- Compliance with privacy regulations

## Troubleshooting

### Common Issues
1. **Iframe Not Loading**
   - Check network connectivity
   - Verify domain access to id.lazytech.ir
   - Ensure no content blockers are active

2. **Dauid Not Generated**
   - Verify iframe is properly placed
   - Check browser console for errors
   - Ensure proper initialization order

## Support
For any issues related to Dauid implementation, contact our support team or check the [SDK Script](/docs/sdk-script) documentation for more details. 