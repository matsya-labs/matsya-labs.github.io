# matsya-labs.github.io

Homepage of Matsya Labs. Plain HTML and CSS, no build step, no JavaScript.

- `index.html` is the whole site.
- `matsya.css` is a copy of `theme/dist/matsya.css` from the theme repo. Replace it when the theme changes.
- `assets/` holds the logo files copied from the logo folder and the social preview image.

Served by GitHub Pages from the `main` branch (Settings → Pages → Deploy from branch, `/ (root)`).

## Custom domain later

1. Add a `CNAME` file containing the bare domain, e.g. `matsyalabs.in`.
2. At the DNS provider: `A` records for the apex to GitHub Pages (185.199.108.153, .109.153, .110.153, .111.153)
   and a `CNAME` record `www → matsya-labs.github.io`.
3. In Settings → Pages set the custom domain and enable "Enforce HTTPS".
4. Change the `og:image` URL in `index.html` to the new domain.
