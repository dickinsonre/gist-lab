<div align="center">

# 🔮 Gist Lab

### Live browser for every dickinsonre public gist — search, preview & run 60+ SWMM tools in-page

![Live Demo](https://img.shields.io/badge/Live%20Demo-dickinsonre.github.io%2Fgist--lab-00b4d8?style=for-the-badge&logo=github)
![License](https://img.shields.io/github/license/dickinsonre/gist-lab?color=success&style=for-the-badge)
![Gists Indexed](https://img.shields.io/badge/Gists-64%2B-f39c12?style=for-the-badge&logo=github)
![Zero Build](https://img.shields.io/badge/Build-None%20Needed-27ae60?style=for-the-badge)

</div>

---

## 🌈 What This Is

**Gist Lab** is a single-page app (`index.html`) that calls the GitHub API live, at the moment you load the page, to pull every public gist from [gist.github.com/dickinsonre](https://gist.github.com/dickinsonre) — currently 64+ SWMM/EPANET/ICM tools, explainers, and side projects — and renders them as a searchable, previewable, runnable-in-page catalog [page:4].

> ⚠️ This is **not** a static curated list. Nothing here is hardcoded — the app talks to GitHub's REST API on every visit.

## 🚀 Live Demo

> 🔗 **[Open Gist Lab →](https://dickinsonre.github.io/gist-lab/)**

## 🔑 About the Rate Limit / Token Panel

GitHub's anonymous API quota is 60 requests/hour **per IP**, shared by everyone behind that IP (corporate NATs, VPNs, shared crawler infra) [page:4]. If you land on an empty state reading **"GitHub API rate limit reached,"** that's why — it's not broken, it's a shared quota running dry.

- The app degrades gracefully: you'll see a clear error message, never a silent failure.
- Click the **token panel** to paste a personal GitHub token and unlock a much higher authenticated rate limit (5,000 req/hour) for your own session.
- No token is stored server-side — it's used client-side only for that browsing session.

## 🛠️ Features

- 🔎 **Live GitHub API fetch** — always shows your current gist list, no manual updates needed
- 📋 **Search & preview** — filter and inspect gists without leaving the page
- ⚡ **Run in-page** — launch supported SWMM/hydraulic tools directly
- 🔑 **Token escape hatch** — bypass anonymous rate limits with a personal token
- 🧱 **Zero backend, zero build** — pure static `index.html` on GitHub Pages

## 📦 Tech Stack

| Layer | Technology |
|---|---|
| 🧱 Structure | HTML5 |
| ⚙️ Logic | Vanilla JavaScript (GitHub REST API, Fetch) |
| 🌐 Hosting | GitHub Pages |

## 🧩 Getting Started

```bash
git clone https://github.com/dickinsonre/gist-lab.git
cd gist-lab
open index.html
```

Works standalone locally too — just be aware local testing shares the same anonymous rate limit as everyone else on your network.

## 📄 License

MIT — see [LICENSE](https://github.com/dickinsonre/gist-lab/blob/main/LICENSE).

---

<div align="center">

Made with 💧 by **[Robert Dickinson](https://github.com/dickinsonre)**

</div>
