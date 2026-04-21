Personal academic website, hosted on GitHub Pages at https://HazelCC.github.io.

Built with Jekyll (which GitHub Pages builds for you automatically on push).

## Structure

- `index.html` — home page (profile, research, miscellanea)
- `blog.html` — index of blog posts, auto-generated from `_posts/`
- `photography.html` — photo gallery, driven by `_data/photos.yml`
- `_posts/` — one Markdown file per blog post, named `YYYY-MM-DD-slug.md`
- `_layouts/` — shared HTML shells (`default.html` adds the nav; `post.html` wraps blog posts)
- `_data/photos.yml` — list of photos shown on the photography page
- `_config.yml` — site-wide variables (name, bio, email, social links)
- `stylesheet.css` — all styles
- `images/` — static images

## Editing

- **Your name, bio, links, email** — edit `_config.yml`. Changes propagate to every page.
- **Research intro & publications** — edit `index.html`. Look for `{{...}}` placeholders.
- **Profile photo** — drop a file into `images/` and update `profile_photo:` in `_config.yml`.
- **New blog post** — add a file like `_posts/2026-05-01-my-post.md` with front matter:

  ```markdown
  ---
  layout: post
  title: "My post title"
  date: 2026-05-01
  ---

  Post body in Markdown.
  ```
- **New photo** — put the file under `images/` and add an entry to `_data/photos.yml`.

## Preview locally

Install dependencies once:

```
bundle install
```

Then run:

```
bundle exec jekyll serve
```

Open http://localhost:4000.

If you don't want to install Ruby/Bundler, you can still push to GitHub and let GitHub Pages build it — just note that you won't see a preview locally.

## Attribution

Template based on [Jon Barron's website](https://github.com/jonbarron/jonbarron.github.io).
