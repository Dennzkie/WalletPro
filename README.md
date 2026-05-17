# WalletPro — HCI2 Web Reporting Site

**Course:** HCI2 – Human-Computer Interaction
**School:** Partido State University, Goa, Camarines Sur

---

## 📁 File Structure

```
walletpro-hci2/
│
├── index.html                  ← Home Page (edit this first)
│
├── pages/
│   ├── data-gathering.html     ← Data Gathering Page
│   └── results.html            ← Results & Recommendations Page
│
├── css/
│   ├── global.css              ← Navbar, Footer, shared styles (DON'T edit unless needed)
│   └── home.css                ← Home page specific styles
│
├── js/
│   └── main.js                 ← Navbar toggle, scroll animations
│
└── assets/
    ├── images/
    │   ├── team/               ← PUT TEAM PHOTOS HERE (jpg/png/webp)
    │   └── prototype/          ← PUT PROTOTYPE SCREENSHOTS HERE
    └── docs/                   ← PUT PDF FILES HERE (consent form, workbooks)
```

---

## ✅ Checklist: What To Customize

### Home Page (`index.html`)

- [ ] Add Figma prototype embed URL (see comment inside `index.html`)
- [ ] Add Figma prototype link for the "Try the Prototype" button
- [ ] Fill in team leader name and role
- [ ] Fill in 4 member names and roles
- [ ] Add team photos (put files in `assets/images/team/`)

#### How to add a photo:
Replace this block:
```html
<div class="photo-placeholder">
  <div class="ph-avatar">👤</div>
  <span>Add Photo</span>
</div>
```
With:
```html
<img src="assets/images/team/your-photo.jpg" alt="Member Name" class="card-photo" />
```
*(For pages/ directory, use `../assets/images/team/your-photo.jpg`)*

#### How to add Figma embed:
1. Open Figma → Click Share on your prototype
2. Copy the prototype link
3. Change `figma.com/proto/` to embed format:
   - **From:** `https://www.figma.com/proto/XXXX/...`
   - **To:** `https://www.figma.com/embed?embed_host=share&url=https://www.figma.com/proto/XXXX/...`
4. Uncomment the `<iframe>` in `index.html` and put your embed URL in `src=""`
5. Delete the `<div class="prototype-placeholder">` block

---

### Data Gathering (`pages/data-gathering.html`)

- [ ] Add consent form (embed PDF or paste content)
- [ ] Add respondent profiles/summary
- [ ] Add Heuristic Evaluation Workbooks (1 per member)
- [ ] Add usability testing survey/instruments
- [ ] Add testing photos (put in `assets/images/`)

#### How to embed a PDF:
```html
<iframe src="../assets/docs/consent-form.pdf" width="100%" height="500px"></iframe>
```

---

### Results & Recommendations (`pages/results.html`)

- [ ] Add summary of usability testing results
- [ ] Add key issues identified
- [ ] Add discussion of findings
- [ ] Add recommendations
- [ ] Add suggested design improvements
- [ ] Attach Heuristic Evaluation Workbook PDF

---

## 🌐 Deployment

After completing all pages, deploy via one of:
- **GitHub Pages** — Push to GitHub, enable Pages in Settings
- **Netlify** — Drag and drop the `walletpro-hci2/` folder at netlify.com/drop
- **Vercel** — Connect GitHub repo or drag and drop

---

## 🎨 Brand Colors

| Color | Hex | Used for |
|-------|-----|---------|
| Blue Primary | `#1A72FA` | Navbar, buttons, accents |
| Blue Dark | `#0f55c7` | Hover states, gradients |
| Background | `#ECF3FB` | Page background |
| White | `#ffffff` | Cards |
| Gray | `#9aa3b0` | Muted text |

To change any color, edit the `:root` variables in `css/global.css`.
