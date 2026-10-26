<div align="center">

# Privacy QR Generator

[![pages-build-deployment](https://github.com/R0mb0/Privacy_qr_generator/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/R0mb0/Privacy_qr_generator/actions/workflows/pages/pages-build-deployment)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/76428162f748495db74a6a2ec8375e19)](https://app.codacy.com/gh/R0mb0/Privacy_qr_generator/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/R0mb0/Privacy_qr_generator)
[![Open Source Love svg3](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](https://github.com/R0mb0/Privacy_qr_generator)
[![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/license/mit)
[![Donate](https://img.shields.io/badge/PayPal-Donate%20to%20Author-blue.svg)](http://paypal.me/R0mb0)

A completely client-side, privacy-respecting QR code generator built with HTML, Tailwind CSS, and Vanilla JS. Features a modern UI, fully offline execution, deep graphical customization, and multiple export formats. 100% front-end, zero server interaction.

<div align="center">
  <a href="http://paypal.me/R0mb0">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://github.com/R0mb0/Support_the_dev_badge/blob/main/Badge/SVG/Support_the_dev_badge_Dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://github.com/R0mb0/Support_the_dev_badge/blob/main/Badge/SVG/Support_the_dev_badge_Light.svg">
      <img alt="Saved you time? Support the dev" src="https://github.com/R0mb0/Support_the_dev_badge/blob/main/Badge/SVG/Support_the_dev_badge_Default.svg">
    </picture>
  </a>
</div>

</div>

<div align="center">

## 👉 [Click here to test the page!](https://r0mb0.github.io/Privacy_qr_generator/) 👈

[![01.png](https://github.com/R0mb0/Privacy_qr_generator/blob/main/Readme_Imgs/01.png)](https://r0mb0.github.io/Privacy_qr_generator/)

[![02.png](https://github.com/R0mb0/Privacy_qr_generator/blob/main/Readme_Imgs/02.png)](https://r0mb0.github.io/Privacy_qr_generator/)

</div>

---

## 🚀 Features

- 100% client-side QR generation (privacy-first)
- Modern, responsive UI with rounded components and Tailwind CSS
- Auto/Manual theme (light/dark) via user preference or OS setting
- Multi-input support: Link, Text, Image, and Video (with size checks)
- Live preview and deep customization (dots, corners, colors, background)
- Add custom text around the QR code borders
- Export to PNG, WEBP, and PDF with adjustable quality/scale
- Fully offline capable: all fonts, icons, and libraries are stored locally

---

## 🛠️ How it works

1. The app takes user input (URL, formatted text, or local files via FileReader).
2. It passes the data to `qr-code-styling` to compute the matrix and render the canvas.
3. Custom CSS and Flexbox are applied to render the external borders and user-defined labels around the generated QR code.
4. When exporting, it uses `html2canvas` to capture a pixel-perfect snapshot of the customized DOM element for PNG/WEBP exports, and `jsPDF` for PDF generation.

---

## 🔒 Privacy & Security

- 100% front-end: all data processing, including file conversion, happens locally in your browser.
- No files, strings, or logs are uploaded to any server.
- Dragged images and videos are processed as local Base64 data strings.

---

## ⚡ Getting Started

1. Download or clone this repository.
2. Make sure the following folder structure is intact:
   - `index.html`
   - `css/` (Contains Inter font CSS and Phosphor icons)
   - `fonts/` (Contains local `.woff2` font files)
   - `js/` (Contains Tailwind, QR Code Styling, html2canvas, and jsPDF)
3. Open `index.html` in any modern browser. 

No server or backend installation is required.

---

## 🧭 Usage

- **Input Data:** Select the tab for your desired content (Link, Text, Image, Video) and enter your data or drag & drop a file.
- **Customize:** Use the right-side panel (or bottom on mobile) to adjust the style (square to rounded), background color, dot color, and add custom text to any of the 4 borders.
- **Export:** Select your desired format (PNG, WEBP, PDF) and quality scale.
- **Save:** Click the "Download" button to save your file.
- **Reset:** Click the "Reset" button next to download to clear all fields and start over.

---

## 🧩 Project Structure

```
Privacy_qr_generator/
├─ index.html         # Main app shell, logic, and JS processing
├─ css/               # Tailwind config, local Inter CSS, and Phosphor Icons
├─ fonts/             # Local Inter font binaries (.woff2)
└─ js/                # Pre-packaged local libraries
├─ tailwindcss.js
├─ qr-code-styling.js
├─ html2canvas.min.js
└─ jspdf.umd.min.js
```

---

## ✅ Browser Support

- Chrome, Firefox, Edge, Safari — latest versions recommended.
- Desktop and mobile supported. Layout intelligently adapts to screen size.

---

## ⚠️ Limitations & Notes

- **Data Limits:** QR Code standard data limits apply (max ~2.9 KB). If an uploaded image or video exceeds this limit, the app will block the generation to prevent outputting an unscannable QR code.
- **Rendering:** Border text rendering relies on `html2canvas` parsing the DOM. Specific advanced browser font-rendering anomalies might occasionally appear on mobile.

---

## 🙌 Credits & Inspiration

- [Tailwind CSS](https://tailwindcss.com)
- [Phosphor Icons](https://phosphoricons.com)
- [qr-code-styling](https://github.com/kozakdenys/qr-code-styling)
- [html2canvas](https://html2canvas.hertzen.com/)
- [jsPDF](https://github.com/parallax/jsPDF)


<a href="https://github.com/R0mb0/Crafted_with_AI">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/R0mb0/Crafted_with_AI/blob/main/Badge/SVG/CraftedWithAIDark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://github.com/R0mb0/Crafted_with_AI/blob/main/Badge/SVG/NotMadeByAILight.svg">
    <img alt="Crafted with AI" src="https://github.com/R0mb0/Crafted_with_AI/blob/main/Badge/SVG/NotMadeByAIDefault.svg">
  </picture>
</a>
