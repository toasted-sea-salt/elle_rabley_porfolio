# Elle Rabley — Portfolio Site

A multi-page personal portfolio built for elite consulting and graduate program recruitment.

## Structure

```
elle-portfolio/
├── index.html              → Home / Landing
├── about/index.html        → About, Education, Skills, Certifications
├── experience/index.html   → Research & Professional Roles
├── involvement/index.html  → Campus Leadership & Community
├── projects/index.html     → Campus Commons, LetterLoft, CardLanes
├── contact/index.html      → Connect
└── assets/
    ├── style.css           → Shared design system
    ├── main.js             → Shared JS (nav, scroll reveals)
    ├── favicon.svg         → ER initials favicon
    └── elle-rabley-resume.pdf  ← ADD YOUR RESUME HERE
```

## Setup

### 1. Add your resume PDF
Drop your resume PDF into `assets/` named `elle-rabley-resume.pdf`.
It's linked from the Experience page and Contact page.

### 2. Add your headshot
In `about/index.html`, find the `bio-photo-placeholder` div and replace with:
```html
<img src="../assets/headshot.jpg" alt="Elle Rabley" />
```
Add a professional headshot at `assets/headshot.jpg` (compress to under 300KB).

### 3. Update LinkedIn URL
Search for `linkedin.com/in/ellerabley` across all files and replace with your actual LinkedIn URL.

### 4. Deploy to GitHub Pages

**Option A — Same repository (subfolder):**
Push the entire `elle-portfolio/` folder to your repo. In GitHub Settings → Pages, set source to the folder containing `index.html`.

**Option B — Root of repo:**
Copy all contents of `elle-portfolio/` to the root of your repository.

**Option C — Vercel (recommended for custom domain):**
1. Push to a GitHub repo
2. Import to Vercel — it'll auto-detect as a static site
3. No build step needed

## Customization

### Accent color
In `assets/style.css`, change `--accent: #B07D4A;` to your preferred color.
Current palette is a warm camel/bronze. Alternatives:
- Dusty rose: `#C4887A`
- Deep sage: `#5C6B5E`
- Warm gold: `#C9A84C`

### Typography
Fonts are loaded from Google Fonts in `style.css`. Current pairing:
- **Headings**: Playfair Display (serif)
- **Body**: DM Sans (sans-serif)

## Design Notes

- Mobile-first responsive — tested at 375px, 768px, 1200px+
- Sticky navigation with active state detection
- Scroll-triggered reveal animations on all sections
- Open Graph meta tags on every page for clean LinkedIn previews
- All external links open in `_blank` with `rel="noopener"`
- No JavaScript frameworks — pure HTML/CSS/JS, zero build step
- Loads in under 1s (no images beyond headshot)

## Pages at a Glance

| Page | Route | Key Content |
|------|-------|-------------|
| Home | `/` | Hero, feature grid, stats strip |
| About | `/about/` | Bio, education, skills, certifications |
| Experience | `/experience/` | 4 research/professional roles, resume download |
| Involvement | `/involvement/` | 7 leadership roles, citizen science |
| Projects | `/projects/` | Campus Commons (featured), LetterLoft, CardLanes |
| Contact | `/contact/` | Email, LinkedIn, availability status |

---

Built with intent. © 2026 Elle Rabley.
