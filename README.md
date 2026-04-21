Personal academic website, hosted on GitHub Pages at https://HazelCC.github.io.

## Preview locally

```
python3 -m http.server
```

Then open http://localhost:8000.

## Editing

- Content lives in `index.html`. Search for `{{...}}` placeholders (name, bio, affiliation, email, links, research intro, and example entries for publications / micropapers / talks / academic service / teaching) and fill them in.
- The template ships with Jon Barron's profile photo at `images/JonBarron.jpg`. Drop your own photo in `images/` and update the two references in `index.html` (the `<a href>` and the `<img src>`) to point to it.
- There is no dedicated "News" section in the template; if you want one, add an `<h2>News</h2>` block above the Research section following the same table pattern.
- Styling lives in `stylesheet.css`.

## Attribution

Template based on [Jon Barron's website](https://github.com/jonbarron/jonbarron.github.io).
