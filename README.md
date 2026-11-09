# MonoPack Pro

Turn a website zip (or a React/Vite source project) into **one self-contained HTML file**, right in your browser. Installable as an app (PWA), works on phones, tablets and desktops.

## Features
- Inlines CSS, JavaScript, images, fonts and CSS `url()` assets
- Compiles React + TypeScript + Tailwind projects in the browser
- Embeds files loaded by JavaScript (up to about 24 MB)
- Live preview and one-tap download
- Private: nothing is uploaded
- Installable, with offline support for normal zips

## Files
```
index.html            app + landing page (guide, limits, rules, terms, FAQ)
manifest.webmanifest  install info
sw.js                 offline cache
favicon.svg, icons/   app icons
```

## Publish from your phone (GitHub Pages)
1. Create a new repository on github.com (public).
2. Tap **Add file, then Upload files** and add everything from this folder, keeping the `icons` folder.
3. Commit, then open **Settings, then Pages**. Choose branch `main` and folder `/ (root)`, and save.
4. After a minute your link appears. Open it and use **Add to home screen**.

Other hosts: Netlify Drop, Cloudflare Pages or any static host work the same way. Service workers need **https**.

## Limits
Static sites and built `dist` folders work fully. React/Vite source projects work but need internet to open the result. Vue, Svelte, Next.js, Angular and backend apps are not supported.

## Privacy
Conversion runs locally. Helper libraries load from public CDNs (Google Fonts, cdnjs, jsDelivr, esm.sh).

## License
MIT
