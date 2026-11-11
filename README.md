# tAIlored

**Know your shoe size in every brand before you order.**
اعرف مقاسك في كل ماركة قبل أن تطلب.

tAIlored is a product concept for Egypt and MENA: measure your feet with your phone camera and a bank card, then get the size each brand actually makes for you, with a confidence score, and shop only what's in stock in that size.

![tAIlored](assets/og.png)

## Try it

- **Website:** `index.html` (English and Arabic)
- **Interactive prototype:** `app/` — 32 screens, a working sizing engine and every edge case clickable. On a desktop, the demo panel lets you change the lighting and steadiness before a scan; on a phone, open it from **Demo controls**.

> This is a concept prototype. The scan is simulated, so nothing uses your camera and no real orders or payments are made. Brand names belong to their owners and are used only to demonstrate sizing; there is no affiliation.

## What the prototype shows

- **Confidence threshold:** scans below 80% confidence take a separate path that explains why and asks for a rescan.
- **Sizing engine:** brand-specific allowances, size steps (including thirds), and width handling that borrows room from a longer size.
- **Fit feedback loop:** rating a pair as tight or loose shifts every future recommendation for that brand.
- **Phone-number sign-in** with a one-time code, rate limiting and a guest mode that migrates data to an account.
- **Privacy controls:** export your data as a JSON file, or delete measurements or the whole account.
- **Arabic and English**, with right-to-left layout.

## How it was built

1. Business requirements document: market, segments, functional requirements
2. User research in FigJam: personas, empathy maps, journey map, sign-in flowchart
3. Design system in Figma: 28 components, 133 variants, Arabic-ready type, dark mode
4. Interactive prototype in plain HTML, CSS and JavaScript (no build step)

## Run it locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

## Settings

At the bottom of `index.html`, in `CONFIG`:

- `formspreeId` — a free [Formspree](https://formspree.io) form ID to turn on the waitlist form
- `linkedin`, `github` — profile and repo links

---

Product concept and design by **Hatem Ghazy**.
