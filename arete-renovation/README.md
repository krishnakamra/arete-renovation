# Arete Renovation Website

A complete, premium, 16-page static website for **Arete Renovation** — Toronto's premier home renovation and remodeling company.

---

## File Structure

```
arete-renovation/
├── index.html                  ← Homepage (hero, about, services, gallery, testimonials)
├── about.html                  ← Company story, values, timeline
├── contact.html                ← Contact form (Netlify), Google Maps, info
├── services.html               ← Master services hub
├── thank-you.html              ← Post-form submission confirmation
│
├── home-improvement.html       ← Interior service page
├── basement-renovation.html    ← Interior service page
├── bathroom-renovation.html    ← Interior service page
├── painting.html               ← Interior service page
├── carpentry.html              ← Interior service page
├── flooring-tiling.html        ← Interior service page
├── handyman-services.html      ← Interior service page
│
├── deck.html                   ← Exterior service page
├── fence.html                  ← Exterior service page
├── custom-sheds.html           ← Exterior service page
├── custom-pergola.html         ← Exterior service page
├── gazebo-installation.html    ← Exterior service page
│
├── css/
│   └── global.css              ← All shared styles, animations, design tokens
├── js/
│   └── global.js               ← Navbar, mobile menu, scroll reveal, counters, lightbox
├── images/
│   └── logo.svg                ← ← ← ADD YOUR LOGO HERE
│
├── netlify.toml                ← Netlify config (headers, cache, redirects)
├── robots.txt                  ← SEO robots file
└── sitemap.xml                 ← XML sitemap for search engines
```

---

## ⚡ Deploy to Netlify (Drag & Drop — 60 seconds)

1. **Add your logo** — Place your SVG file at `images/logo.svg`
2. Go to **[netlify.com](https://netlify.com)** and sign in
3. On the dashboard, drag the entire `arete-renovation/` folder onto the "drag and drop" deploy zone
4. Your site is live instantly at a `*.netlify.app` URL
5. Go to **Domain Settings** → add `areterenovation.ca` as a custom domain
6. Netlify auto-provisions a free SSL certificate (HTTPS) within minutes

### Netlify Form Setup
The contact form on `contact.html` uses Netlify Forms (no backend needed).
- Forms are captured automatically on first deploy
- Go to **Netlify Dashboard → Forms** to view submissions and set up email notifications
- Submissions redirect to `thank-you.html`

---

## 🌩 Deploy to Cloudflare Pages

1. Push the folder to a **GitHub repository**
2. In the Cloudflare dashboard go to **Pages → Create a project**
3. Connect your GitHub repo
4. Set:
   - **Build command:** *(leave blank — static site)*
   - **Build output directory:** `/` (root)
5. Deploy — Cloudflare assigns a `*.pages.dev` URL
6. Add `areterenovation.ca` as a custom domain in the Pages settings

---

## 🖼 Logo Setup

Replace `images/logo.svg` with your actual SVG logo file.

The logo is referenced in every page's navbar and footer as:
```html
<img src="images/logo.svg" alt="Arete Renovation Logo"/>
```

Recommended logo dimensions:
- **Navbar height:** 44px tall (width auto)
- **Footer height:** 48px tall (width auto)
- Use an SVG with transparent background
- Ensure the logo works on dark (#0A0A0A) backgrounds — light or gold-coloured artwork works best

---

## 🎨 Design System

| Token | Value |
|---|---|
| Primary Gold | `#C5A059` |
| Light Gold | `#E6C786` |
| Dark Gold | `#8A6D3B` |
| Background Black | `#0A0A0A` |
| Background Dark | `#111111` |
| Card Background | `#161616` |
| Body Text | `#F5F5F5` |
| Muted Text | `#A0A0A0` |
| Heading Font | Cinzel (Google Fonts) |
| Body Font | Montserrat (Google Fonts) |

---

## 📱 Features

- ✅ Fully mobile-responsive with hamburger menu
- ✅ Smooth scroll-reveal animations (IntersectionObserver)
- ✅ Animated stat counters
- ✅ Image gallery with lightbox
- ✅ Sticky scrolled navbar with backdrop blur
- ✅ Gold gradient hover effects throughout
- ✅ FAQ accordions on all service pages
- ✅ Netlify form with honeypot spam protection
- ✅ Google Maps embed (dark-filtered to match theme)
- ✅ SEO meta tags, canonical URLs, sitemap.xml, robots.txt
- ✅ Security headers via netlify.toml
- ✅ Static asset cache headers (1 year)
- ✅ No build step required — pure HTML/CSS/JS

---

## 📞 Contact Details Embedded Throughout

- **Phone:** 437-990-0355
- **Email:** areterenovation16@gmail.com
- **Website:** areterenovation.ca
- **Service Area:** Greater Toronto Area, ON

---

*Built with Tailwind CSS CDN, Cinzel + Montserrat via Google Fonts, and Vanilla JavaScript.*
