# SMmyth — Silver Merchant Portfolio Website

A personal portfolio website for **Dumbreni Stewart**, a Web Master based in Harare, Zimbabwe. The site showcases skills, education, work experience, and projects in a clean multi-page layout with a responsive navigation bar.

---

## 📄 Project Description

SMmyth is a multi-page static portfolio website built with plain HTML, CSS, and JavaScript. It features four main sections:

- **Home (Hero)** — Introduction with a profile image and a call-to-action button.
- **About** — Bio, skills with proficiency percentages, education timeline, and work experience.
- **Projects** — A card-based gallery of completed projects with GitHub links.
- **Contact** — A contact form and social/email links.

The design uses a dark background image (`images/bg.jpg`) across all pages, a frosted-glass sticky navbar, and a consistent aqua/white color palette.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Page structure and content |
| CSS3 | Styling, layout (Flexbox/Grid), and responsive design |
| JavaScript (Vanilla) | Mobile navbar toggle functionality |
| Google Fonts — Poppins | Typography |

> No frameworks, build tools, or external dependencies are required. The site runs entirely in the browser.

---

## 📁 File Structure

```
/
├── hero.html           # Home / landing page
├── about.html          # About Me page
├── projects.html       # Projects showcase page
├── contact.html        # Contact form page
│
├── hero.css            # Styles for the hero/home page
├── about.css           # Styles for the About page
├── projects.css        # Styles for the Projects page
├── contacts.css        # Styles for the Contact page
├── navbar.css          # Shared responsive navbar styles
│
├── javascript.js       # Navbar hamburger toggle script
│
└── images/
    ├── bg.jpg                          # Background image (used on all pages)
    ├── 1 (6).png                       # Profile photo (hero page)
    ├── Screenshot 2026-03-27 212249.png  # Project 1 screenshot
    ├── Screenshot 2026-03-27 212348.png  # Project 2 screenshot
    └── Screenshot 2026-03-27 212500.png  # Project 3 screenshot
```

---

## ⚙️ Setup Instructions

No build process or package installation is needed.

### 1. Clone or Download the Repository

```bash
git clone https://github.com/dumbrenistewart-lang/web-tech.git
cd web-tech
```

Or download the ZIP from GitHub and extract it.

### 2. Add Your Images

Make sure the `images/` folder exists in the same directory as the HTML files and contains:
- `bg.jpg` — the background image used across all pages
- `1 (6).png` — your profile photo
- The three project screenshot files referenced in `projects.html`

### 3. Open in a Browser

Simply open `hero.html` in any modern web browser:

```bash
# On Windows
start hero.html

# On macOS
open hero.html

# On Linux
xdg-open hero.html
```

No local server is required since the site uses no server-side code or ES modules.

### 4. (Optional) Serve with a Local Dev Server

For a smoother development experience with auto-reload, you can use the VS Code **Live Server** extension or Python's built-in HTTP server:

```bash
# Python 3
python -m http.server 8000
```

Then visit `http://localhost:8000/hero.html` in your browser.

---

## ✏️ Customisation Guide

| What to change | Where to edit |
|---|---|
| Your name and bio | `about.html` — `.container` section |
| Hero introduction text | `hero.html` — `.intro` div |
| Skill percentages | `about.html` — `.skill-percent` spans |
| Projects (title, description, links) | `projects.html` — `.card` divs |
| Contact email | `contact.html` — `form action` attribute and the anchor tag |
| Background image | Replace `images/bg.jpg` (keep the same filename) |
| Brand/logo name | All HTML files — `.navbar-logo` anchor text |

---

## 🐛 Known Issues & Notes

- The contact form uses `mailto:` which relies on the user's default email client. For a proper backend form submission, consider integrating a service like [Formspree](https://formspree.io) or [EmailJS](https://www.emailjs.com).
- `hero.html` contains a minor HTML typo (`/<div`) that should be corrected to `<div`.
- `contact.html` has an extra unclosed `</div>` tag that can be safely removed.
- The navbar hover rule in `navbar.css` has a typo: `2px solis` should be `2px solid`.

---

## 👤 Author

**Dumbreni Stewart**
- Email: dumbrenistewart@gmail.com
- GitHub: [dumbrenistewart-lang](https://github.com/dumbrenistewart-lang/web-tech.git)
- Location: Harare, Zimbabwe

---

## 📜 License

This project is open source and available for personal and educational use.
