# Δ = THE OBSERVER + Solar  
**Live Bell-State CHSH Quantum Demo — 100% Offline PWA**

> **S = 2.8281 > 2**  
> **Spooky action at a distance — in your pocket.**

---

## Live Demo  
[https://observer-delta.github.io](https://observer-delta.github.io)

**Installable on iOS & Android**  
No internet needed after first load.

---

## Features

| Feature | Status |
|-------|--------|
| Real-time CHSH Bell inequality simulation | Done |
| Noise slider (γ) with decoherence | Done |
| Live NOAA solar X-ray flux | Done |
| 30-minute flare probability | Done |
| **100% offline** via local Pyodide | Done |
| **PWA** — Add to Home Screen | Done |
| **Mobile donation** (no QR needed) | Done |
| Auto-retry on network failure | Done |

---

## How to Use

1. **Slide noise** → watch entanglement decay  
2. **Tap "Collapse Now"** → measure CHSH  
3. **S > 2** → **SPOOKY LINK SURVIVED** (pulsing green)  
4. **Tap "Support the Spooky Link"** → donate via PayPal (mobile-friendly)

---

## Tech Stack

- **Pyodide** (local, unzipped via GitHub Actions)  
- **NumPy** in-browser  
- **NOAA GOES X-ray API** (dual endpoints)  
- **PWA** with `manifest.json` + icons  
- **GitHub Pages** + `.nojekyll`

---

## Install as App

1. Open in **Safari** or **Chrome**  
2. Tap **Share** → **Add to Home Screen**  
3. Launch — works **offline forever**

---

## Support the Mission

> *"Every collapse is a vote against local realism."*

[Support the Spooky Link](https://paypal.me/yourpaypalusername)  
*(Replace with your PayPal link in `index.html`)*

---

## Badge (Copy to your README)

```svg
<svg width="320" height="110" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="grad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#0f0">
        <animate attributeName="stop-color" values="#0f0;#00f;#0f0" dur="3s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" stop-color="#00f">
        <animate attributeName="stop-color" values="#00f;#0f0;#00f" dur="3s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>
  <rect width="320" height="110" fill="#000" rx="18" stroke="#333" stroke-width="2"/>
  <text x="160" y="38" font-family="monospace" font-size="20" fill="url(#grad)" text-anchor="middle" filter="url(#glow)">
    SPOOKY SOLAR OBSERVER
  </text>
  <text x="160" y="62" font-family="monospace" font-size="13" fill="#0f0" text-anchor="middle">
    Δ = Quantum + Sun
  </text>
  <text x="160" y="82" font-family="monospace" font-size="11" fill="#aaa" text-anchor="middle">
    S = 2.828 > 2 | NOAA-Resilient | Pyodide
  </text>
  <text x="160" y="98" font-family="monospace" font-size="9" fill="#666" text-anchor="middle">
    Auto-Retry • Dual Endpoint • Mobile-Ready
  </text>
</svg>
