# 🔍 IETF Document Fixer

> *Thanks to the marvels of modern display technology, you now own a glorious 4K ultrawide monitor capable of rendering the entire surface area of a small continent. IETF chose to celebrate this achievement by rendering all document text in a cozy little column huddled on the left-hand side — as if it's afraid of the dark and refuses to move away from the nearest wall. The other 75% of your screen sits there, empty, judging you.*
>
> *This browser extension fixes that. You're welcome.*

---

## What does it do?

Injects a small CSS fix on every page under `https://datatracker.ietf.org/doc/*` that constrains the `.card-body` elements to a sensible reading width, centres them, and left-aligns the text — so documents look like documents, not ASCII art panoramas.

```css
.card-body {
  max-width: 600px;
  margin: 0 auto;
  text-align: left;
}
```

## Before & After

### Before — content cowering in the corner

![Before: content huddled in the top-left, leaving most of the screen a vast, empty wasteland](https://github.com/user-attachments/assets/470378e8-d3ef-4678-8978-fbb722cb99e5)

### After — centred, readable, civilised

![After: content centred at a comfortable reading width](https://github.com/user-attachments/assets/fbab3b5e-f40c-451b-8d38-98057a218226)

---

## Installation (Microsoft Edge / Chrome)

> The extension uses **Manifest V3** and works in any Chromium-based browser (Edge, Chrome, Brave, etc.).

1. **Download or clone** this repository to your machine.
2. Open your browser and navigate to the extensions page:
   - **Edge:** `edge://extensions`
   - **Chrome:** `chrome://extensions`
3. Enable **Developer mode** (toggle in the top-right corner).
4. Click **Load unpacked**.
5. Select the root folder of this repository (the one containing `manifest.json`).
6. The extension will appear in your browser toolbar. Visit any `https://datatracker.ietf.org/doc/` page and enjoy text that doesn't require a panoramic display to read.

---

## Contributing

PRs welcome. If you find other IETF layout crimes that need fixing, open an issue.

## License

[MIT](LICENSE)
