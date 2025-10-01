# Dakia Chat Widget CDN

A lightweight chat widget that can be easily integrated into any website using our CDN.

## Quick Start

Add the following script tag to your HTML page to integrate the Dakia chat widget:

```html
<script
  src="https://cdn.jsdelivr.net/gh/NerdFlow/dakia-chat-widget-cdn/widget.iife.js"
  data-client-id="200"
  data-primary-color="#343434"
  data-secondary-color="#00ff00"
></script>
```

## Installation

### Basic Integration

1. Add the script tag to your HTML `<head>` or before the closing `</body>` tag:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Your Website</title>
  </head>
  <body>
    <!-- Your website content -->

    <!-- Dakia Chat Widget -->
    <script
      src="https://cdn.jsdelivr.net/gh/NerdFlow/dakia-chat-widget-cdn/widget.iife.js"
      data-client-id="200"
      data-primary-color="#343434"
      data-secondary-color="#00ff00"
    ></script>
  </body>
</html>
```

2. Replace `"your-client-id"` with your actual client ID provided by Dakia.

## Configuration

The widget can be configured using data attributes on the script tag:

### Required Attributes

- `data-client-id`: Your unique client identifier (required)

### Optional Attributes

You can customize the widget colors by adding color data attributes:

```html
<script
  src="https://cdn.jsdelivr.net/gh/NerdFlow/dakia-chat-widget-cdn/widget.iife.js"
  data-client-id="200"
  data-primary-color="#343434"
  data-secondary-color="#00ff00"
></script>
```

#### Available Configuration Options

| Attribute              | Default     | Description                                |
| ---------------------- | ----------- | ------------------------------------------ |
| `data-client-id`       | _required_  | Your unique client identifier              |
| `data-primary-color`   | `"#007bff"` | Primary color for the widget (hex color)   |
| `data-secondary-color` | `"#6c757d"` | Secondary color for the widget (hex color) |

## Examples

### Basic Usage

```html
<script
  src="https://cdn.jsdelivr.net/gh/NerdFlow/dakia-chat-widget-cdn/widget.iife.js"
  data-client-id="200"
  data-primary-color="#343434"
  data-secondary-color="#00ff00"
></script>
```

### Custom Configuration

```html
<script
  src="https://cdn.jsdelivr.net/gh/NerdFlow/dakia-chat-widget-cdn/widget.iife.js"
  data-client-id="200"
  data-primary-color="#ff6b6b"
  data-secondary-color="#4ecdc4"
></script>
```

### Multiple Environments

#### Development

```html
<script
  src="https://cdn.jsdelivr.net/gh/NerdFlow/dakia-chat-widget-cdn/widget.iife.js"
  data-client-id="200"
  data-primary-color="#343434"
  data-secondary-color="#00ff00"
></script>
```

#### Production

```html
<script
  src="https://cdn.jsdelivr.net/gh/NerdFlow/dakia-chat-widget-cdn/widget.iife.js"
  data-client-id="prod-client-id"
  data-primary-color="#007bff"
  data-secondary-color="#6c757d"
></script>
```

## CDN Information

- **CDN Provider**: jsDelivr
- **Base URL**: `https://cdn.jsdelivr.net/gh/NerdFlow/dakia-chat-widget-cdn/`
- **Main File**: `widget.iife.js`
- **Cache**: Files are cached by jsDelivr for optimal performance

### Version Pinning

For production environments, you may want to pin to a specific version:

```html
<!-- Pin to a specific commit -->
<script
  src="https://cdn.jsdelivr.net/gh/NerdFlow/dakia-chat-widget-cdn@{commit-hash}/widget.iife.js"
  data-client-id="your-client-id"
></script>

<!-- Pin to a specific tag/release -->
<script
  src="https://cdn.jsdelivr.net/gh/NerdFlow/dakia-chat-widget-cdn@v1.0.0/widget.iife.js"
  data-client-id="your-client-id"
></script>
```

## Browser Support

The Dakia chat widget supports all modern browsers:

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## Performance

- **File Size**: Optimized for minimal bundle size
- **Loading**: Asynchronous loading to prevent blocking page render
- **Caching**: Leverages browser and CDN caching for fast subsequent loads

## Troubleshooting

### Widget Not Appearing

1. Check that your `data-client-id` is correct
2. Ensure the script tag is properly formatted
3. Check browser console for any JavaScript errors
4. Verify your domain is authorized for the client ID

### Common Issues

- **Script blocked**: Check if ad blockers or content security policies are blocking the script
- **CORS errors**: Ensure your domain is whitelisted for the client ID
- **Multiple widgets**: Only one widget instance per page is supported

## Security

- All communications are encrypted using HTTPS
- The widget respects your website's Content Security Policy (CSP)
- No sensitive data is stored in browser localStorage

**Note**: Replace `"your-client-id"` with the actual client ID provided by Dakia support.
