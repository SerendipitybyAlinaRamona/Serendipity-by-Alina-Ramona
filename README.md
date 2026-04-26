# ✦ Serendipity by Alina Ramona
### Astrologie & Consiliere în Dezvoltare Personală

> Website bilingv (română / engleză) pentru practica de astrologie, consiliere și cărțile Alinei Ramona.
> Bilingual (Romanian / English) website for Alina Ramona's astrology practice, counseling, and books.

**Live site:** `https://YOUR-GITHUB-USERNAME.github.io/serendipity-alina-ramona/`

---

## 🗂️ What's Inside

One single file — `index.html` — contains the entire website. No frameworks, no database, no dependencies to maintain.

| Page | How to reach it | Contents |
|---|---|---|
| **Home** | Default / Logo click | Hero, Services, About, Booking (Calendly), Testimonials, Contact |
| **Books** | "Cărți / Books" in nav | Petals of Becoming trilogy — all 3 books with Amazon links |
| **Articles** | "Articole / Articles" in nav | Blog list — add new articles manually (see below) |

---

## 🚀 Deploying / Updating on GitHub Pages

### First-time setup
1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Create a new repository named `serendipity-alina-ramona` — set it to **Public**
3. Upload `index.html` and `README.md` via **Add file → Upload files**
4. Go to **Settings → Pages → Source: Deploy from branch → main / root → Save**
5. Wait 1–2 minutes → your site is live ✅

### Updating the site (any future change)
1. Open your repository on GitHub
2. Click `index.html` → click the **pencil icon ✏️** to edit
3. Select all (`Ctrl+A`), delete, paste the new version
4. Click **Commit changes** → **Commit changes** again in the popup
5. Site updates automatically within ~1 minute

---

## 📅 Calendly (Booking)

Your Calendly is already embedded and live at:
```
https://calendly.com/serendipitybyalinaramona
```

Romanian visitors see the calendar in Romanian automatically (`?locale=ro` is already set).

### To change the Calendly link in future
Search for `calendly.com/serendipitybyalinaramona` in `index.html` and replace with your new URL.

### To change session types shown above the calendar
Find the `booking-options` section in `index.html` and edit the four `booking-type` blocks — change the glyph, title, or duration as needed.

---

## 📚 Books Page — Petals of Becoming

The three books are already configured with your real Amazon links:

| Book | Amazon Link | Status |
|---|---|---|
| Petals of Growth | `amazon.com/gp/product/B0GY5PJB9X` | Live ✅ |
| Petals of Self-Love | `amazon.com/gp/product/B0GY98VZGT` | Live ✅ |
| Petals of Abundance | — | Coming Soon ribbon shown |
| Full series | `amazon.com/dp/B0GY8SBHTD` | Live ✅ |

### When Petals of Abundance is published
1. Open `index.html` and find the third book card (search for `Petals of Abundance`)
2. Remove the two `coming-soon-ribbon` lines
3. Replace the `<span class="book-soon">` lines with a button like the other two:
```html
<a href="https://www.amazon.com/gp/product/YOUR-ASIN" target="_blank" class="book-btn">
  <span data-ro>Găsește pe Amazon →</span><span data-en>Find on Amazon →</span>
</a>
```

---

## ✍️ Articles Page — Adding New Posts

The articles page is a simple manual list. No CMS needed.

### To add a new article
Open `index.html`, find the `articles-list` section, and **copy this block** — paste it above the first existing article (so newest appears first):

```html
<div class="article-item fade-in">
  <div>
    <div class="article-meta">
      <span>DD Lun YYYY</span>
      <span class="article-tag" data-ro>Astrologie</span>
      <span class="article-tag" data-en>Astrology</span>
    </div>
    <div class="article-title" data-ro>Titlul articolului în română</div>
    <div class="article-title" data-en>Article title in English</div>
    <p class="article-excerpt" data-ro>Primul paragraf sau introducere în română — 2-3 propoziții.</p>
    <p class="article-excerpt" data-en>Opening paragraph or introduction in English — 2-3 sentences.</p>
  </div>
  <div class="article-arrow">→</div>
</div>
```

**Tag options** — change the tag text to match your topic:
- `Astrologie` / `Astrology`
- `Dezvoltare Personală` / `Personal Development`
- `Sinastrie` / `Synastry`
- `Revenire Solară` / `Solar Return`
- `Reflecții` / `Reflections`

---

## ✏️ Common Edits

### Change your email address
Search for `serendipitybyalinaramona@gmail.com` — it appears twice. Replace both.

### Add WhatsApp or social media links
Find this block in the Contact section and uncomment / fill in:
```html
<!-- Add WhatsApp:
<a href="https://wa.me/40XXXXXXXXX" class="contact-link" target="_blank">
  <span class="icon">◉</span>
  <span class="lbl">WhatsApp</span>
</a>
-->
```
Remove the `<!--` and `-->` and fill in your phone number (format: country code + number, no spaces or dashes).

### Add your photo to the About section
Upload a photo named `alina.jpg` to the GitHub repository, then find the `chart-wheel` div in `index.html` and replace it with:
```html
<img src="alina.jpg" alt="Alina Ramona"
  style="width:280px;height:280px;object-fit:cover;border-radius:50%;border:1px solid rgba(212,168,83,0.3);">
```

### Add real client testimonials
Find the three `testimonial` blocks in `index.html` and replace the placeholder text with real quotes. Keep the `data-ro` and `data-en` tags — one for the Romanian version, one for English.

---

## 🌍 Romanian SEO — Getting Found on Google

The site already includes Romanian-language meta tags and keywords. To go further:

### 1. Google Search Console (free — do this first)
- Go to [search.google.com/search-console](https://search.google.com/search-console)
- Add your GitHub Pages URL as a property
- Google gives you a `<meta name="google-site-verification">` tag — paste it inside `<head>` in `index.html`
- Submit your URL for indexing

### 2. Google Business Profile (free)
- Go to [business.google.com](https://business.google.com)
- Add your practice — this makes you appear in local Romanian Google searches
- Suggested categories: **Astrolog**, **Consilier în dezvoltare personală**

### Keywords already in the site
`astrologie harta natala Romania` · `consultatie astrologie online` · `sinastrie compatibilitate` · `consilier dezvoltare personala` · `astro relocare` · `astrolog online romana` · `petals of becoming` · `petals of growth` · `petals of self love`

---

## 🔧 Tech Stack

| Technology | Purpose | Cost |
|---|---|---|
| HTML / CSS / JavaScript | Entire website — single file | Free |
| GitHub Pages | Hosting | Free forever |
| Google Fonts (Cormorant Garamond + Jost) | Typography | Free |
| Calendly (free plan) | Session booking | Free |
| Google Search Console | SEO indexing | Free |
| Google Business Profile | Local Romanian search visibility | Free |

**Total monthly cost: €0**

---

## 📁 File Structure

```
serendipity-alina-ramona/
├── index.html     ← The entire website (edit this for all changes)
├── README.md      ← This file
└── alina.jpg      ← Optional: add your photo here
```

---

*✦ Serendipity by Alina Ramona · Astrologie & Consiliere în Dezvoltare Personală*
*serendipitybyalinaramona@gmail.com*
