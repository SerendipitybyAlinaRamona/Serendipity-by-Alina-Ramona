# ✦ Serendipity by Alina Ramona
### Astrologie & Consiliere în Dezvoltare Personală

> Website bilingv (română / engleză) pentru practica de astrologie și consiliere a Alinei Ramona.  
> Bilingual (Romanian / English) website for Alina Ramona's astrology and personal development counseling practice.

---

## 🌐 Live Site

Once deployed on GitHub Pages, your site will be available at:
```
https://YOUR-GITHUB-USERNAME.github.io/serendipity-alina-ramona/
```

---

## 📋 What's Included

A single `index.html` file containing the complete website:

| Section | Content |
|---|---|
| **Hero** | Name, tagline, CTA button — bilingual |
| **Services** | Natal chart, Synastry, Solar Return, Astro Relocation, Personal Development Counseling, Transits & Progressions |
| **About** | 20-year background, licensed counselor credential |
| **Booking** | Calendly embed area (see setup below) |
| **Testimonials** | 3 placeholder testimonials |
| **Contact** | Email link (and slots for WhatsApp, Instagram, Facebook) |
| **Footer** | Copyright |

---

## 🚀 Deploying to GitHub Pages (Free Hosting)

### Step 1 — Create a GitHub Account
Go to [github.com](https://github.com) and sign up. It's free.

### Step 2 — Create a New Repository
1. Click the **+** button → **New repository**
2. Name it: `serendipity-alina-ramona`
3. Set it to **Public**
4. Click **Create repository**

### Step 3 — Upload the File
1. On the repository page, click **Add file** → **Upload files**
2. Drag and drop `index.html` (and this `README.md` if you like)
3. Click **Commit changes**

### Step 4 — Enable GitHub Pages
1. Go to **Settings** (top tab of your repository)
2. Scroll to **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Choose branch: **main**, folder: **/ (root)**
5. Click **Save**
6. Wait 1–2 minutes, then your site is live ✅

---

## 📅 Setting Up Calendly (Free Booking)

Calendly's free plan is sufficient for this site.

### Step 1 — Create Your Calendly Account
Go to [calendly.com](https://calendly.com) and sign up for free.

### Step 2 — Create Event Types
Create one event type for each service, for example:
- `Hartă Natală` — 90 minutes
- `Sinastrie` — 75 minutes
- `Consiliere în Dezvoltare Personală` — 60 minutes
- `Revenire Solară` — 60 minutes
- `Astro-Relocare` — 60 minutes

### Step 3 — Get Your Calendly Username
Your Calendly URL looks like: `https://calendly.com/alina-ramona`  
Your username is the part after `calendly.com/` → in this case `alina-ramona`

### Step 4 — Add Calendly to the Site
Open `index.html` in a text editor. Find this block (around line 290):

```html
<div id="calendly-embed-container">
  <!-- CALENDLY PLACEHOLDER ... -->
  <div class="calendly-placeholder">
    ...
  </div>
</div>
```

**Replace the entire block** with these two lines:

```html
<div class="calendly-inline-widget" data-url="https://calendly.com/YOUR-USERNAME" style="min-width:320px;height:630px;"></div>
<script type="text/javascript" src="https://assets.calendly.com/assets/external/widget.js" async></script>
```

Replace `YOUR-USERNAME` with your actual Calendly username.

**To show Romanian interface for Romanian visitors**, use:
```
https://calendly.com/YOUR-USERNAME?locale=ro
```

---

## 🌍 Romanian SEO — Getting Found on Google

The site already includes Romanian-language SEO meta tags. To improve discoverability further:

### 1. Register on Google Search Console (Free)
- Go to [search.google.com/search-console](https://search.google.com/search-console)
- Add your GitHub Pages URL as a property
- Verify ownership (Google will give you a meta tag — paste it inside `<head>` in `index.html`)
- Submit your sitemap (just your URL, since it's a single page)

### 2. Create a Google Business Profile (Free)
- Go to [business.google.com](https://business.google.com)
- Add your practice — this helps you appear in local Romanian searches
- Category: **Astrolog** and/or **Consilier psihologic**

### 3. Keywords Already in the Site
The site is optimized for searches like:
- `astrologie harta natala Romania`
- `consultatie astrologie online`
- `sinastrie compatibilitate`
- `consilier dezvoltare personala`
- `astro relocare`
- `astrolog online romana`

---

## ✏️ Customizing the Site

All edits are made directly in `index.html` using any text editor (Notepad, VS Code, etc.).

### Change the Email Address
Search for `contact@serendipity-alina.ro` and replace with your actual email address (appears twice — in the `href` and as display text).

### Add WhatsApp / Social Media
Find this comment block near the Contact section:
```html
<!-- Uncomment and fill in when you have WhatsApp/social: -->
```
Remove the `<!--` and `-->` around the links you want, and fill in your phone number / social handles.

### Add Your Real Photo
Replace the zodiac wheel in the About section with your photo by adding after the `<div class="about-visual">` tag:
```html
<img src="alina-ramona.jpg" alt="Alina Ramona" style="width:280px; height:280px; object-fit:cover; border-radius:50%; border: 1px solid rgba(200,169,110,0.3);">
```
Upload `alina-ramona.jpg` to the same GitHub repository folder.

### Replace Placeholder Testimonials
Find the `<section id="testimonials">` section and edit the three testimonial blocks with real client quotes (with their permission).

### Add a Custom Domain (Optional, Still Free)
If you register a free domain via [eu.org](https://nic.eu.org) (takes ~2–4 weeks for approval):
1. In your GitHub repository, create a file named `CNAME` (no extension)
2. Inside it, write only your domain: `serendipity-alina.ro`
3. Point your domain's DNS to GitHub Pages (GitHub's documentation explains this step)

---

## 🗂️ File Structure

```
serendipity-alina-ramona/
├── index.html        ← The entire website (one file)
├── README.md         ← This file
└── alina-ramona.jpg  ← (optional) Add your photo here
```

---

## 🔧 Tech Stack

| Technology | Purpose | Cost |
|---|---|---|
| HTML / CSS / JavaScript | Website — single file, no framework | Free |
| GitHub Pages | Hosting | Free forever |
| Google Fonts (Cormorant Garamond + Jost) | Typography | Free |
| Calendly (free plan) | Booking | Free |
| Google Search Console | SEO indexing | Free |
| Google Business Profile | Local Romanian search | Free |

**Total monthly cost: €0**

---

## 📞 Support

This site was built as a single self-contained HTML file — no database, no server, no dependencies to maintain. If you need to make changes and get stuck, the entire site is in one file and any text editor can open it.

---

*✦ Serendipity by Alina Ramona · Astrologie & Consiliere în Dezvoltare Personală*
