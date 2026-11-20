# Personal site

A one-page site with projects and writing, hosted free on GitHub Pages.

## Edit your profile and projects

Open `site.json` on GitHub, click the pencil icon, change the text between the quotes, and click **Commit changes**. The site updates in about a minute.

- `linkedin` / `instagram`: a full profile link or just your handle (`@you`).
- `links`: any other links, each as `{ "label": "...", "url": "..." }`.
- `photo` (optional): add `"photo": "me.jpg"` and upload `me.jpg` next to `index.html`.
- `projects`: copy a `{ ... }` block for each project. `live` is a deployed link (GitHub Pages, Vercel, Netlify…), `code` is the GitHub repo. Leave either as `""`.

Keep the commas between items. If the page says it can't load `site.json`, a missing or extra comma is the usual cause.

## Add writing

Go to the `writing` folder, click **Add file → Upload files**, and drop in a `.md`, `.txt` or `.pdf` file. It shows up on the site automatically.

- Name files like `2026-11-19-my-essay.md` so they get a date and sort newest first.
- In a Markdown file, the first line `# My Title` becomes the title. For a summary line, start the file with:

```
---
title: My Title
date: 2026-11-19
summary: One sentence shown in the list.
---
```

If the site is on a custom domain, set `"github": "your-username/your-repo"` in `site.json` so new writing is found automatically.

## Turn on GitHub Pages

Repo **Settings → Pages → Build and deployment**: Source "Deploy from a branch", branch `main`, folder `/ (root)`. Your site will be at `https://<username>.github.io/<repo>/`.
