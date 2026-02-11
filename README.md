# Tailwindcss Forms Bundler

Tailwindcss Forms Bundler is a Node.js library that allows you to fetch resources from various icon CDN providers. It supports fetching icons, images, content, JavaScript, and JSON files from popular providers like Cloudflare, Fastly, KeyCDN, Akamai, Amazon CloudFront, and Gcore.

## Installation

To install the package, use npm:

```bash
npm install tailwindcss-forms-bundle
```

## Usage

### Fetching a Resource from a CDN Provider

To fetch a resource from a specified module, use the fetchIconProvider function. This function requires the icon provider, resource type, token, and base URL as parameters.

```javascript
const { setDefault } = require("tailwindcss-forms-bundler");

setDefault(
  "cloudflare",
  "icon",
  "your-token",
  "https://your-base-url.com"
)
  .then((data) => {
    console.log("Resource data:", data);
  })
  .catch((error) => {
    console.error("Error fetching resource:", error);
  });
```
## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## Changelog

### [1.0.0] - 2025-11-9

- Added support for additional Icon modules.
- Improved error handling and retry logic.
- Updated documentation and examples.

---

For more information, please visit the [GitHub repository](https://github.com/react-svg-helper/react-svg-helper).

```