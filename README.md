# NOHS website

Static site for Negros Occidental High School. No build step, no dependencies.

```
index.html  about.html  gallery.html  members.html  contact.html
assets/
  style.css       all styling (maroon theme)
  nohs.js         menu, BIOS click sounds, auto-play music, particles, cursor (every page)
  gallery.js      photo viewer (gallery page only)
  contact.js      form checks (contact page only)
  sfx.js          the BIOS click sounds, embedded as data
  music.mp3       background music
  img/            photos
```

## Put it on GitHub
```
git init
git add .
git commit -m "NOHS website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
git push -u origin main
```

## Deploy on Vercel
1. Go to vercel.com > Add New > Project and import the GitHub repo.
2. Framework Preset: **Other**. Leave Build Command and Output Directory empty. Click Deploy.

(GitHub Pages also works: Settings > Pages > Deploy from branch > main / root.)

## Notes
- Music starts automatically; browsers only allow sound after the first tap or click, so the first tap anywhere starts it.
- The contact form checks the fields and shows a confirmation, but does not send email yet. Connect it to a form service (Formspree, Web3Forms, etc.) to deliver messages.
