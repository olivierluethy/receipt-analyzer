<div align="center">
  <img src="logo.png" alt="Receipt Analyzer logo" width="140" />
  <h1>Receipt Analyzer</h1>
  <p><b>Turn a photo of a receipt into clean, structured data — right in your browser.</b><br/>A single-file receipt scanner that reads merchant, date, line items, taxes and total using the Claude Vision API.</p>
  <p>
    <a href="LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-blue.svg"></a>
    <img alt="HTML5" src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white">
    <img alt="CSS3" src="https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white">
    <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black">
    <img alt="Claude" src="https://img.shields.io/badge/Claude%20Vision-D97757?logo=anthropic&logoColor=white">
  </p>
</div>

---

**Browser-based receipt scanner that turns a photo of a receipt into structured
data** — using the Claude Vision API. Drop in a receipt image and get back the
merchant, date, line items, taxes and total as clean, structured output you can
copy or export. Everything runs in a **single HTML file** — no build step, no
backend, no framework.

## Features

- **Image → structured data.** Extracts merchant, date, individual line items,
  quantities, prices, tax and total from a receipt photo.
- **Powered by Claude Vision.** Uses Anthropic's Claude model to read even messy,
  crumpled or low-contrast receipts.
- **Zero install.** One `receipt-analyzer.html` file — open it in any modern browser.
- **Client-side only.** The image goes straight from your browser to the Claude API;
  there is no server in between.

## Getting started

1. Open `receipt-analyzer.html` in your browser (double-click, or serve it locally).
2. Paste your **Anthropic API key** when prompted (get one at
   [console.anthropic.com](https://console.anthropic.com)).
3. Upload or drag in a receipt image.
4. Read back the extracted, structured result.

> **Note on the API key:** the key is used directly from the browser to call the
> Claude API. Use a key you control and rotate it if you share the page publicly.

## How it works

The page sends the uploaded image to the Claude Vision API with a prompt that asks
for the receipt broken down into structured fields, then renders the model's
response. Because it is a single static file, you can host it anywhere (GitHub
Pages, Netlify, any static host) or just run it locally.

## Tech

Plain HTML, CSS and JavaScript · Claude Vision API (Anthropic).

## License

Released under the [MIT License](LICENSE) © 2026 Olivier Lüthy. You're free to use, modify and distribute this
software, including commercially, as long as the copyright notice and license are included.

## Author

Built by **Olivier Lüthy** — [GitHub](https://github.com/olivierluethy).
