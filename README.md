# Zebra Films site

One-page site for Zebra Films LLC. Plain HTML/CSS/JS, no build step.

```
zebra-films/
  index.html        the whole site
  assets/
    temi.jpg        portrait for the About section (optional)
    thumbs/         project thumbnails (optional)
```

## 1. Fill in your details

Open `index.html` and find the `CONFIG` and `PROJECTS` blocks near the bottom (marked "EDIT HERE").

- `CONFIG.email`: your Zebra Films email (currently `temi@zebrafilms.us`).
- `CONFIG.reel`: a YouTube or Vimeo link to your reel. Until it's set, the reel shows "New reel coming soon".
- Each project's `video`: paste the YouTube or Vimeo link. Unlisted Vimeo links (`vimeo.com/123456/abcdef`) work. Projects with a video get a play button and open in a player.
- Each project's `thumb`: path to an image, such as `assets/thumbs/nike.jpg`. Without one, the card shows a title card.

## 2. Save your assets before leaving Adobe Portfolio

Your old site is hosted on Adobe Portfolio. Before you cancel it or move the domain:

1. Download your About photo and project stills, and save them into `assets/`.
2. Collect the video links for each project (Edit each project in Adobe Portfolio and copy the embed source).
3. Check these names from the old site: "Chuckwunonso Dureke" (director of Plantain & Proverbs) was carried over as written.

## 3. Publish

Any static host works. Two free options:

- **Netlify:** drag the `zebra-films` folder onto app.netlify.com/drop, then add your domain under Domain settings.
- **GitHub Pages:** push the folder to a repo, enable Pages on the `main` branch, then add your domain under Settings > Pages.

At your domain registrar, point the domain at the host using the DNS records the host gives you. HTTPS is issued automatically.

## 4. Point the old site at the new one

When temiolutunmbi.com is rebuilt as your creator site, link to Zebra Films from it, and redirect old portfolio paths so existing links keep working:

| Old URL | New URL |
|---|---|
| temiolutunmbi.com/work | yourdomain.com/#work |
| temiolutunmbi.com/commercial | yourdomain.com/#work |
| temiolutunmbi.com/personal | yourdomain.com/#work |

On Netlify, put these in a `_redirects` file on the temiolutunmbi.com site.
