# ✨ AI Image Enhancer

A modern, responsive web app that upscales and enhances images using the **Picsart AI API** — with an automatic **free offline fallback** powered by HTML5 Canvas. Zero dependencies, zero build steps.

![GitHub stars](https://img.shields.io/github/stars/yourusername/ai-image-enhancer?style=social)
![License](https://img.shields.io/badge/license-MIT-blue)
![HTML](https://img.shields.io/badge/built%20with-HTML%2FCSS%2FJS-orange)

---

## 🚀 Live Demo

> Host it free on GitHub Pages — see [Getting Started](#getting-started) below.

---

## ✨ Features

- **AI Upscaling (2×, 4×, 8×)** via the Picsart Upscale API
- **Interactive Before/After Slider** — drag to compare original vs enhanced
- **Free Offline Fallback** — works without any API key using progressive Canvas upscaling
- **Dark / Light Mode** — persisted across sessions
- **Clipboard Paste** — paste images directly with Ctrl+V / ⌘V
- **Sample Presets** — try it instantly with built-in demo images
- **Image Stats** — dimensions and mode displayed after enhancement
- **Copy to Clipboard** — copy the enhanced image with one click
- **Direct Download** — lossless PNG download
- **Zero Dependencies** — pure HTML, CSS, and Vanilla JS

---

## 🛠️ Getting Started

### Run Locally

Just open `index.html` in any modern browser — no install required.

Or serve it locally:

```bash
# Python 3
python -m http.server 8000

# Node.js (npx)
npx serve .
```

Then visit `http://localhost:8000`.

### (Optional) Add Your Picsart API Key

1. Get a free API key at [picsart.io/developers](https://picsart.io/developers)
2. Paste it into the API Key field on the page, **or** set `DEFAULT_API_KEY` inside `index.html`:

```js
const DEFAULT_API_KEY = "your-key-here";
```

> ⚠️ Use your **API Key**, not an OAuth access token — a token will cause an auth error.

No key? No problem — the app falls back to the free offline upscaler automatically.

---

## 🌐 Deploy to GitHub Pages (Free)

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under **Build and deployment → Source**, select **Deploy from a branch**
4. Choose branch: `main`, folder: `/ (root)`
5. Click **Save** — your site will be live in ~1 minute

---

## 📁 Project Structure

```
ai-image-enhancer/
├── index.html      # The entire app (self-contained)
├── README.md
├── .gitignore
└── LICENSE
```

---

## 🔒 Privacy

Images are sent to the Picsart API for processing (when a key is provided) and are never stored on your device. When using the offline fallback, all processing happens entirely in your browser — no data leaves your machine.

---

## 📄 License

MIT — free to use, modify, and distribute.
