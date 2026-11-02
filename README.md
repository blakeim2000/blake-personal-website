# blake-personal-website

A personal site: two static pages, no build step, no dependencies, no JavaScript.

| file | what's in it |
| --- | --- |
| `index.html` | **About me** — the landing page |
| `startups.html` | **Data for startups** |
| `styles.css` | The whole design, shared by both pages |

## Editing it

Copy lives in the `<main>` of each page as plain paragraphs and lists. Edit the
text, save, refresh the browser.

Colours are tokens on `:root` at the top of `styles.css`, with the dark-mode set
right underneath. Adding a page means copying one of the HTML files and adding a
link to the `<nav>` in *both* existing pages — the nav is hand-written, since
there's no templating.

## Viewing it

Double-click `index.html`, or serve it:

```
python -m http.server 8000     # then http://localhost:8000
```

## Deploying

GitHub Pages serves this as-is from the default branch, root folder: there is
nothing to build. Settings -> Pages -> Source: "Deploy from a branch", branch
`main`, folder `/ (root)`.
