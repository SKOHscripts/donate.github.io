# donate.github.io

<a href="https://html-preview.github.io/?url=https://github.com/SKOHscripts/donate.github.io/blob/main/donate%2Fredirect.html" target="_blank">
  <img src="https://github.com/SKOHscripts/donate.github.io/blob/main/donate/buymeacoffee.png?raw=true" width="100">
</a>

---

# Bitcoffee Donation Page

A simple, stylish, **Bitcoin donation page** built with HTML, CSS, and JavaScript.
Designed for developers and open-source enthusiasts to receive donations via Bitcoin.

![Preview](donate/demonstration.gif)

---

## Live Demo

Check out a working version here:
[https://github.com/SKOHscripts/donate.github.io](https://github.com/SKOHscripts/donate.github.io)

---

## Features

* Stylish orange-dark “dev” theme
* Coffee ☕ + Bitcoin ₿ icons with glowing effect
* QR code generated locally (no external trackers)
* Automatic language detection (EN, FR, ES, DE, IT, PT)
* Click-to-copy Bitcoin URI
* Buttons to open wallet, Bitcoin.org, and Lightning Network
* Fully responsive and scrollable on small screens

---

## Setup / Customization

1. **Clone the repository**:

```bash
git clone https://your-username.github.io/your-repo
cd your-repo
```

2. **Edit the Bitcoin URI** in `index.html`:

```javascript
const texts = {
  uri: "bitcoin:?lno=YOUR_OWN_BITCOIN_ADDRESS_HERE",
  en: { title: "...", subtitle: "...", devMessage: "...", thanksMessage: "...", copied: "Copied! ☕" },
  // other languages...
};
```

Replace `"YOUR_OWN_BITCOIN_ADDRESS_HERE"` with your own Bitcoin address or LNURL.

3. **Deploy to GitHub Pages**:

* Go to your repository → Settings → Pages → Select `main` branch and `/root` folder → Save.
* Wait a few minutes. Your donation page will be available at:

```
https://your-username.github.io/your-repo
```

4. **Optional**: Update the README screenshot to reflect your own page.

---

## License

MIT License – feel free to reuse and modify.

---
