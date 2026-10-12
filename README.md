# lastlight.victorvandi.com

Website for **Last Light**: home page, privacy policy and terms of use. Plain HTML and CSS, no build step.

| Page | URL |
|---|---|
| Home | https://lastlight.victorvandi.com/ |
| Privacy policy (for Google Play) | https://lastlight.victorvandi.com/privacy/ |
| Terms of use | https://lastlight.victorvandi.com/terms/ |

## Deploy on GitHub Pages
1. The repo must be **public** (GitHub Pages on a free account only works for public repos).
2. Repo → **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main`, folder `/ (root)` → Save.
3. Settings → Pages → **Custom domain**: `lastlight.victorvandi.com` → Save. (The `CNAME` file in this repo already contains it.)
4. Namecheap → victorvandi.com → **Advanced DNS → Add new record**: type `CNAME`, host `lastlight`, value `engr-vandi.github.io.`
5. Wait until Settings → Pages says the DNS check passed, then tick **Enforce HTTPS**.
6. Open https://lastlight.victorvandi.com/privacy/ on your phone and check for the padlock.

`.nojekyll` tells GitHub Pages to serve the files as they are. `404.html` is used automatically for missing pages.

## When the app is live on Google Play
Replace both `<span class="btn primary" aria-disabled="true">…Coming soon…</span>` buttons in `index.html` with:

```html
<a class="btn primary" href="https://play.google.com/store/apps/details?id=com.victorvandi.lastlight">Get it on Google Play</a>
```

## Keep the privacy policy true
If the app changes what it collects (ads, analytics, accounts, removing the Google Fonts download), update `privacy/index.html` and its effective date, and the Data safety form in Play Console.
