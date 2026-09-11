# stanislavdurilla.com — source files

A small static site: no build step, no frameworks. Three files types only —
`index.html`, `style.css`, and one `.html` file per article inside `articles/`.

## Publish it on GitHub Pages (free, ~5 minutes)

1. Create a new **public** GitHub repository — name it anything, e.g. `site`
   (or `<your-github-username>.github.io` if you want it at the root of your
   own username domain).
2. Upload all the files in this folder to the repository, keeping the
   `articles/` folder structure intact.
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`,
   branch `main`, folder `/ (root)`. Save.
5. GitHub will give you a live URL within a minute or two, typically
   `https://<username>.github.io/<repo-name>/`.
6. Paste that URL into the "Featured" section of your LinkedIn profile, or
   into your headline/About section as a link.

## Editing content later

- **Add a new article**: copy any file in `articles/` as a template, edit the
  headline, kicker, meta line, and body paragraphs, then add a matching
  `<a class="dispatch">` entry to the list in `index.html`.
- **Update your bio**: edit the "About" section directly in `index.html`.
- **Change colours/fonts**: everything is controlled from the `:root`
  variables at the top of `style.css`.

## Optional: a custom domain

If you'd rather use your own domain (e.g. `stanislavdurilla.com`) instead of
the default `github.io` address, buy the domain from any registrar, then add
a `CNAME` file with just the domain name in it to the repository root, and
point your registrar's DNS at GitHub Pages following GitHub's custom domain
guide. Not necessary to get started — the free `github.io` link works fine
for LinkedIn.
