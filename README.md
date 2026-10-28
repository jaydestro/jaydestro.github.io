# Jay Gordon's website

A lightweight personal portfolio at <https://jaydestro.github.io/>.

## Local preview

From the repository root, run:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open <http://127.0.0.1:8000>. No package installation or build step is needed.

## Editing and publishing

- Update the bio, featured projects, talks, and links in `index.html`.
- Update the layout, colors, and responsive styles in `styles.css`.
- `favicon.svg` contains the site's icon.

GitHub Pages publishes directly from the root of `main`. Merging changes into
`main` triggers publication; feature branches do not change the live site.

Keep the talks and writing list current: only feature content published within
the last two years, and show the month and year for each item. Prefer the Azure
Cosmos DB Blog, YouTube, Microsoft Reactor, and LinkedIn as sources.

Before publishing, check the page at desktop and mobile widths, navigate links
using the keyboard, and confirm that project and talk links point to the intended
destinations. The site does not use JavaScript, external fonts, analytics, or
third-party widgets.
