# Jay Gordon's website

A lightweight personal portfolio at <https://jaydestro.github.io/>.

## Local preview

From the repository root, run:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open <http://127.0.0.1:8000>. No package installation or build step is needed.

## Editing and publishing

- Update the bio, projects, selected works, talks, and links in `index.html`.
- Update professional experience, technical skills, and career highlights in `resume.html`. Keep `resume.pdf` in sync with the HTML; the page includes print styles and a PDF download.
- Both pages use a circular portrait, name, and title in the header and footer, with resume links in the navigation and footer; keep these shared elements in sync.
- Update the layout and responsive styles in `styles.css`. The blue-and-black palette and gradients are defined as CSS variables in its `:root` block.
- `favicon.svg` contains the site's icon. The header and footer use `headshot-480.webp` for the circular portrait; regenerate the photo variants if you replace it.
- The hero uses a responsive YouTube embed. Update the iframe's video ID and `start` value (in seconds), plus its title, caption, and YouTube link, together.

GitHub Pages publishes directly from the root of `main`. Merging changes into
`main` triggers publication; feature branches do not change the live site.

Keep the talks and writing list current: only feature content published within
the last two years, and show the month and year for each item. Prefer the Azure
Cosmos DB Blog, YouTube, Microsoft Reactor, and LinkedIn as sources.
The homepage section order and navigation are Projects, Blogs, Videos, and
Selected works (`#selected-works`). Blogs (`#blogs`) and Videos (`#videos`) are
separate sections. Each shows exactly five items, newest first, with older
items inside its own `.more-talks-list`. Keep entries simple: source, date, and
linked title.
The native `<details>` expanders work without JavaScript and support keyboard
navigation. Use verified audience metrics when selecting for popularity; do
not imply a popularity ranking without them.
The expanded lists also link to the DEV profile and personal JayGordonAzure
YouTube channel for more writing and videos, including older work.

Before publishing, check the page at desktop and mobile widths, navigate links
using the keyboard, and confirm that project and talk links point to the intended
destinations. The site does not use its own JavaScript, external fonts, or
analytics. The featured video uses YouTube's privacy-enhanced embed domain
(`youtube-nocookie.com`); the player loads third-party content.
