# Mama's Birthday Card 🌸

A beautiful, single-file birthday webpage with falling rose petals, a personal letter, and a photo gallery.

---

## Filling It In

Open `index.html` in any text editor and look for the clearly marked placeholder comments:

| What to find | What to replace it with |
|---|---|
| `<!-- YOUR LETTER HERE — paragraph 1 -->` | Your letter text (plain text or HTML) |
| `<!-- YOUR CLOSING QUOTE HERE -->` | A short, warm closing line |
| `<!-- YOUR NAME HERE -->` | Your name |
| `<!-- YOUR SIGN-OFF HERE -->` | Already has "All my love, always," — edit freely |

### Adding Photos

In the gallery section, each photo slot looks like this:

```html
<div class="gallery-item reveal">
  <div class="gallery-placeholder"> ... </div>
  <div class="photo-overlay"></div>
</div>
```

Replace the inner `<div class="gallery-placeholder">…</div>` with:

```html
<img src="photo1.jpg" alt="Describe the moment" />
```

Put your photo files in the same folder as `index.html`. Supported formats: `.jpg`, `.png`, `.webp`.

---

## Previewing Locally

Just double-click `index.html` — it opens straight in your browser. No server or build step needed.

---

## Deploying to GitHub Pages (free, permanent link)

These steps take about 5 minutes.

### 1 — Create a GitHub repository

1. Go to [github.com/new](https://github.com/new)
2. Name it something like `mamas-birthday` (keep it lowercase, no spaces)
3. Set it to **Public**
4. Click **Create repository** — do NOT add a README via the UI

### 2 — Push the files

Open a terminal (or Git Bash on Windows) in this folder and run:

```bash
git init
git add index.html README.md
git commit -m "Happy birthday, Mama 🌸"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/mamas-birthday.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your GitHub username.

### 3 — Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Source**, choose **Deploy from a branch**
4. Set branch to `main`, folder to `/ (root)`
5. Click **Save**

GitHub will show a green banner with your live URL in about 60 seconds:

```
https://YOUR-USERNAME.github.io/mamas-birthday/
```

That's the link you can text, email, or print as a QR code for her.

---

### Updating the page later

After editing `index.html`, push the changes:

```bash
git add index.html
git commit -m "Updated letter"
git push
```

GitHub Pages updates automatically within a minute.

---

*Made with love.*
