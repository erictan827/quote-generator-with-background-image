# Quote Image Generator

> Turn memorable words into polished, shareable artwork—right in your browser.

[![Live Demo](https://img.shields.io/badge/Live_Demo-Open_App-2ea44f?style=for-the-badge)](https://erictan827.github.io/quote-generator-with-background-image/)
[![GitHub Pages](https://img.shields.io/badge/Hosted_on-GitHub_Pages-222?style=for-the-badge&logo=github)](https://pages.github.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

Quote Image Generator is a lightweight React web app for pairing quotations with beautiful nature photography. Search for a public figure, choose a quote, personalize its typography, and export the result as a high-resolution PNG.

## Try it now

**[Launch the live app →](https://erictan827.github.io/quote-generator-with-background-image/)**

No installation or account is required. A modern browser with JavaScript enabled is all you need.

## What you can do

- Search for celebrities and public figures.
- Pick a quote attributed to the selected person.
- Generate a random quote when you want instant inspiration.
- Refresh the canvas with a random nature background from Unsplash.
- Adjust quote font size from 12 px to 72 px.
- Choose any quote color with the built-in color picker.
- Download the finished composition as a 3840 × 2160 PNG.
- Use the responsive browser interface on desktop or mobile.

## How to use it

1. Open the [live app](https://erictan827.github.io/quote-generator-with-background-image/).
2. Type a celebrity's name and select a suggestion, or choose **Random Quote**.
3. Select **Generate Background** until you find an image you like.
4. Adjust the font size and color for readability.
5. Select **Download Image** to save your 4K PNG.

### Tips for better results

- Pick a high-contrast text color for the selected photo.
- Shorter quotes usually produce cleaner social graphics.
- If an API is temporarily unavailable, wait a moment and try again.
- Downloaded images are intended for personal or otherwise properly licensed use. Quote attribution and image licensing remain the user's responsibility.

## How it works

The app combines three external content sources with a client-side image export flow:

1. API Ninjas provides celebrity search suggestions.
2. STANDS4 provides author and random quote results.
3. Unsplash provides random nature photography.
4. `html2canvas` captures the final browser composition and exports a PNG.

The deployed `gh-pages` branch contains the static production build used by GitHub Pages.

## Technology

- React
- Axios
- html2canvas
- API Ninjas Celebrity API
- STANDS4 Quotes API
- Unsplash API
- GitHub Pages

## Local preview

This branch contains a production build, so it can be previewed with any static file server:

```bash
git clone https://github.com/erictan827/quote-generator-with-background-image.git
cd quote-generator-with-background-image
python3 -m http.server 8080
```

Then visit `http://localhost:8080/quote-generator-with-background-image/` if your server preserves the repository base path. For active development, restore the original React source project and keep deployment output separate from source code.

## Privacy and third-party services

Search terms and content requests are sent directly from the browser to the third-party APIs listed above. Their availability, rate limits, privacy practices, and terms apply. This repository does not operate its own backend.

## Known limitations

- The current repository preserves an older compiled demo and does not include the original editable React source tree.
- Results depend on external API availability, quotas, and browser CORS policies.
- Background-image and quotation rights vary; verify the intended use before publishing exported artwork.
- API credentials should not be shipped in browser bundles. See [Security](SECURITY.md) before reusing this build.

## Contributing

Ideas, bug reports, documentation fixes, and pull requests are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) first and use the provided issue templates.

## Support

For help, read [SUPPORT.md](SUPPORT.md) or open a GitHub issue with clear reproduction details. Please do not post secrets or API keys.

## License

The project code is available under the [MIT License](LICENSE). Third-party quotes, images, APIs, trademarks, and other content retain their respective rights and terms.

---

Created by [Eric Tan](https://github.com/erictan827).
