# Polish — Free AI Paper Reviewer for Students

Get reviewer-grade feedback on your academic paper in under two minutes. Eight parallel AI agents examine logic, math, references, arguments, citations, clarity, methods, and writing style.

## Quick Start

1. Download `index.html`
2. Open it in your browser (double-click the file)
3. Paste your Anthropic API key (get one free at [console.anthropic.com](https://console.anthropic.com/settings/keys) — new accounts get $5 in credits)
4. Upload or paste your paper
5. Click **Analyze Paper**

That's it. No install, no server, no terminal, no accounts to create.

## Troubleshooting

If PDF upload doesn't work when opening from `file://`, serve it locally with a one-liner:

```bash
# Python (pre-installed on Mac/Linux)
python3 -m http.server 8000

# Then open http://localhost:8000 in your browser
```

```bash
# Node.js (if you have it)
npx serve .
```

## Cost per Paper

You pay only Anthropic's API cost. No markup, no subscription.

| Model | Short (~5 pp) | Medium (~15 pp) | Long (~30 pp) |
|---|---|---|---|
| Haiku 4.5 | $0.06 | $0.15 | $0.27 |
| Sonnet 4.5 (recommended) | $0.19 | $0.44 | $0.82 |
| Opus 4.5 | $0.31 | $0.73 | $1.37 |

A student revising a medium paper 5 times would spend $1–$4 total with Sonnet.

## Privacy

Your API key stays in your browser's local storage and is sent only to Anthropic's API. Your paper text goes only to Anthropic over HTTPS. There is no server, no analytics, no cookies, no tracking, and no data collection. Everything runs client-side.

## What It Checks

Eight agents run in parallel, each focused on one dimension: logical consistency, mathematical reasoning, internal references, argument completeness, clarity and precision, empirical methods, citations and bibliography, and writing style.

## Customization

Open `index.html` in a text editor. The two arrays to edit are near the top of the `<script>` block: `MODELS` (add/remove Claude models) and `AGENTS` (add/remove review dimensions).

## License

MIT
