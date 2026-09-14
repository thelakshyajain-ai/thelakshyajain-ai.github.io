# thelakshyajain-ai.github.io

Static site served by GitHub Pages at <https://thelakshyajain-ai.github.io/>.

## Layout

```
index.html          landing page
pages/index.html    list of hosted documents (hand-maintained)
pages/*.html        the documents themselves
.nojekyll           disables Jekyll processing
```

## Publishing a page

1. Drop a self-contained `.html` file into `pages/`.
2. Add a matching `<li>` entry to `pages/index.html` — the list does not scan the directory.
3. Commit and push to `main`. Pages rebuilds in under a minute.

## Placeholders to fill before going public

`index.html` contains `TODO_NAME`, `TODO_TAGLINE`, `TODO_BIO`, `TODO_LINKEDIN_URL`,
and `TODO_EMAIL`. `pages/index.html` also carries `TODO_NAME` in its title.

## Notes

- `.nojekyll` must stay. Without it Pages runs Jekyll, which drops files and
  directories whose names begin with an underscore.
- Pages is configured to deploy from the `main` branch, root directory.
- A repo named `<user>.github.io` serves at the account root, not a subpath.
