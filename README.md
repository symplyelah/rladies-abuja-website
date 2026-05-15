# R-Ladies Abuja Website

The official website for R-Ladies Abuja — a local chapter of [R-Ladies Global](https://rladies.org), based in Abuja, FCT, Nigeria.

🌐 Live site: [rladiesabuja.netlify.app](https://rladiesabuja.netlify.app)

## Built With

- [Quarto](https://quarto.org/) — scientific publishing system
- Hosted on [Netlify](https://netlify.com) via GitHub

## Local Development

### Prerequisites

1. Install [R](https://cran.r-project.org/)
2. Install [Quarto CLI](https://quarto.org/docs/get-started/)

### Run Locally

```bash
# Clone the repo
git clone https://github.com/YOUR-ORG/rladies-abuja-website.git
cd rladies-abuja-website

# Preview the site
quarto preview
```

The site will open at `http://localhost:4200`.

### Build

```bash
quarto render
```

Output goes to `_site/`.

## Deploy to Netlify

### Option A: Connect via GitHub (Recommended)

1. Push this repo to GitHub
2. Log in to [Netlify](https://app.netlify.com)
3. Click **Add new site → Import an existing project**
4. Connect your GitHub repo
5. Set build settings:
   - **Build command:** `quarto render`
   - **Publish directory:** `_site`
6. Click **Deploy site** 🚀

Netlify will auto-deploy on every push to `main`.

### Option B: Netlify CLI

```bash
npm install -g netlify-cli
netlify deploy --prod --dir _site
```

## Adding Content

### New Blog Post

```bash
mkdir blog/posts/my-new-post
touch blog/posts/my-new-post/index.qmd
```

Then add YAML front matter:

```yaml
---
title: "My Post Title"
description: "Short description"
date: "2025-04-15"
categories: [tutorial, ggplot2]
author: "Your Name"
---
```

### New Talk

Add a `.qmd` file to `talks/2025/` with details about the talk.

## Community

- 🐦 Twitter: [@RLadiesAbuja](https://twitter.com/RLadiesAbuja)
- 📅 Meetup: [meetup.com/rladies-abuja](https://www.meetup.com/rladies-abuja/)
- 💻 GitHub: [github.com/rladies](https://github.com/rladies)

## License

MIT License — see [LICENSE](LICENSE) for details.

---

Made with 💜 by R-Ladies Abuja
