# Portfolio

Personal site for Shizzel Brown, Accra, Ghana.

Two standalone landing pages, each written for a different client. They are deliberately **not**
linked to each other: a data client who lands on "virtual assistant" downgrades their read, and an
operations client who lands on star schemas assumes you are too technical and too expensive. Each
link gets sent on purpose.

| Path | Page | Sent to |
|---|---|---|
| `/` | Business analyst who builds | Power BI, reporting and analytics clients |
| `/va/` | Executive assistant and content strategist | Founders wanting operations and content run for them |

## Structure

```
index.html      analyst page
va/index.html   operations and content page
va/photo.jpg    source photo (also embedded inline in the page)
```

Each page is one self-contained HTML file. No build step, no dependencies, no framework. Styles,
layout and content all live in the file.

## Local preview

Open either `index.html` in a browser. That is the whole workflow.

## Deploy

GitHub Pages, `main` branch, root folder. Edit, commit, push; Pages rebuilds in about a minute.

## Notes

- Light and dark themes on both pages, driven by the visitor's system setting.
- Responsive to 360px.
- No analytics, no cookies, no third-party requests. Both pages make zero external calls.
- The photo on `/va/` is embedded as a data URI, which is why that page is large. Compressing it
  before any serious traffic is worthwhile.
