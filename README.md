# Color Format Converter

Convert a color between HEX, RGB, HSL, and HSV with a live swatch. No server, no tracking, no third-party scripts.

**Live demo:** https://0xelitesystem.github.io/color-format-converter/

## Use

Open `index.html` in any modern browser, or visit the GitHub Pages link in the repo description.

Paste a color into any field and the other three update instantly:

- **HEX** accepts `#rgb`, `#rrggbb`, with or without the hash.
- **RGB** accepts `rgb(15, 92, 96)` or bare `15, 92, 96`, each channel 0 to 255.
- **HSL** accepts hue 0 to 360 and saturation and lightness as percentages.
- **HSV** (also called HSB) accepts hue 0 to 360 and saturation and value as percentages.

A native color picker and a large swatch give you a live preview, and every row has a copy button. Invalid input is flagged with a red border instead of silently snapping to something wrong.

## Why this exists

Color converters online tend to be ad-heavy pages that phone home on every keystroke. This is the same idea, single file, no analytics, no signup, MIT licensed.

## Privacy

Everything runs in your browser. The colors you type never leave your machine. Verify by viewing the page source or by opening DevTools and watching the network tab, no requests are made.

## Run locally

```bash
git clone https://github.com/0xelitesystem/color-format-converter
cd color-format-converter
# Open index.html in your browser, or:
python -m http.server 8000
```

## Contribute

Issues and PRs welcome:

- More formats (CMYK, named colors, OKLCH)
- Rounding and precision edge cases
- UI improvements (keep it minimal, no frameworks)
- Translations

Don't add: analytics, tracking, external scripts, npm dependencies. The whole point of this tool is no surveillance.

## Build

There is no build. It's a single HTML file.

## License

MIT.

## Related

- [aspect-ratio-calculator](https://github.com/0xelitesystem/aspect-ratio-calculator), simplify dimensions to a ratio and back
- [url-parser-and-query-editor](https://github.com/0xelitesystem/url-parser-and-query-editor), break a URL into parts and edit query params
- [word-and-character-counter](https://github.com/0xelitesystem/word-and-character-counter), count words, characters, and reading time
