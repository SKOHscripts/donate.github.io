# donate.github.io
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
<a href="https://html-preview.github.io/?url=https://github.com/SKOHscripts/donate.github.io/blob/main/donate%2Fredirect.html" target="_blank">
  <img src="https://github.com/SKOHscripts/donate.github.io/blob/main/donate/buymeacoffee.png?raw=true" width="100">
</a>

---

# Fuel the code — Donation Page

A single-file donation page with a **One Dark IDE** ambience and an **iOS-style** card.
Accepts GitHub Sponsors, Bitcoin (Lightning, Silent Payments, on-chain), Monero and Zcash.

![Preview](donate/preview.png)

---

## Live Demo

[https://html-preview.github.io/?url=https://github.com/SKOHscripts/donate.github.io/blob/main/donate%2Fredirect.html](https://html-preview.github.io/?url=https://github.com/SKOHscripts/donate.github.io/blob/main/donate%2Fredirect.html)

---

## Features

* One Dark background with abstract code lines scrolling slowly (shapes only, no readable text; static when *reduced motion* is enabled)
* Frosted-glass card with iOS segmented controls: **Sponsor · Bitcoin · Monero · Zcash**
* Bitcoin sub-options: **Lightning**, **Silent Payments** (BIP-352) and **On-chain** (Native SegWit)
* QR codes generated locally (`qrcode.js`, no external requests or trackers)
* Tap the address to copy it (first and last characters highlighted for checking)
* "Open in wallet" button using `lightning:`, `bitcoin:`, `monero:` and `zcash:` URIs
* Deep links: `redirect.html#lightning`, `#silent`, `#onchain`, `#monero`, `#zcash`, `#sponsor`
* Keyboard (← →) and swipe navigation
* Automatic language detection (EN, FR, ES, DE, IT, PT)

---

## Setup / Customization

1. **Clone the repository**:

```bash
git clone https://github.com/SKOHscripts/donate.github.io
cd donate.github.io
```

2. **Edit the `METHODS` array** at the top of the script in `donate/redirect.html`:

```javascript
const METHODS = [
  { id: 'sponsor',   group: 'sponsor', label: 'GitHub Sponsors', address: 'github.com/sponsors/YOU', uri: 'https://github.com/sponsors/YOU' },
  { id: 'lightning', group: 'bitcoin', label: 'Lightning',       address: 'you@wallet.tld',         uri: 'lightning:you@wallet.tld' },
  { id: 'monero',    group: 'monero',  label: 'Monero',          address: '8…',                     uri: 'monero:8…' },
  // …
];
```

Texts for each method (tag and note) live in the `I18N` object, keyed by the method `id`.

3. **Deploy to GitHub Pages**: Settings → Pages → select the `main` branch and `/root` folder → Save.

---

## License

MIT License – feel free to reuse and modify.

---
