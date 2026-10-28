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
- Update the layout and responsive styles in `styles.css`. The blue-and-black palette and gradients are defined as CSS variables in its `:root` block.
- `favicon.svg` contains the site's icon. `headshot-480` and `headshot-960` (WebP with JPEG fallback) are the hero portrait; regenerate both sizes if you replace the photo.
- The hero uses a small circular portrait and a responsive YouTube embed. Update the iframe's video ID and `start` value (in seconds), plus its title, caption, and YouTube link, together.

GitHub Pages publishes directly from the root of `main`. Merging changes into
`main` triggers publication; feature branches do not change the live site.

Keep the talks and writing list current: only feature content published within
the last two years, and show the month and year for each item. Prefer the Azure
Cosmos DB Blog, YouTube, Microsoft Reactor, and LinkedIn as sources.
Show & Tell keeps three selected highlights visible; additional recent items
go inside `.more-talks-list`. Its native `<details>` expander works without
JavaScript and supports keyboard navigation. Use verified audience metrics when
selecting for popularity; do not imply a ranking without them.

Before publishing, check the page at desktop and mobile widths, navigate links
using the keyboard, and confirm that project and talk links point to the intended
destinations. The site does not use its own JavaScript, external fonts, or
analytics. The featured video uses YouTube's privacy-enhanced embed domain
(`youtube-nocookie.com`); the player loads third-party content.
