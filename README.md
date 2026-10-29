# IAEA Navigator site

Support, privacy, terms, accessibility and account-deletion pages for the IAEA Navigator app, published with GitHub Pages from `main` at https://moore99.github.io/IAEA-Navigator-site/.

## IndexNow

IndexNow tells Bing (and through it DuckDuckGo, Yahoo, Ecosia and Copilot search), Yandex, Seznam and Naver about new or changed pages. Google doesn't use it. After each successful Pages build, `.github/workflows/indexnow.yml` POSTs every page's URL to `https://api.indexnow.org/indexnow`. It's best effort: a failure only logs a warning.

The key is `f8035c948406b6ca62bbb62bfaa6fb81`. It's served from the key file `f8035c948406b6ca62bbb62bfaa6fb81.txt` at the site root and also set as `INDEXNOW_KEY` in the workflow. It's public by design, not a secret. Because the key file sits under `/IAEA-Navigator-site/`, IndexNow only accepts URLs under that path.
