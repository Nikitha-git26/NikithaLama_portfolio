# Nikitha Lama — Portfolio

A responsive, modern single-page portfolio built with **HTML5**, **Tailwind CSS** (via CDN), and **vanilla JavaScript**. Includes a hero section, an about section, a projects grid, a working contact form, and a footer.

---

## Project Structure

```
NikithaLama_Portfolio/
├── index.html    # Page markup (Tailwind CSS via CDN)
├── style.css     # Custom styles: animations, hover effects, badges, scrollbar
├── script.js     # Mobile menu, smooth scrolling, scroll reveal, contact form handler
├── photo.jpeg    # Profile photo
└── README.md
```

---

## Running Locally

No build step or dependencies required — it's a static site.

- **Quick:** double-click `index.html` to open it in a browser.
- **With a local server** (avoids relative-path quirks):
  ```bash
  python -m http.server 5500
  ```
  then visit `http://localhost:5500`.

---

## Deploying to Vercel

1. Push this repo to GitHub (already at [Nikitha-git26/NikithaLama_portfolio](https://github.com/Nikitha-git26/NikithaLama_portfolio)).
2. Go to [vercel.com](https://vercel.com) → **Add New Project** → import the repo.
3. Framework preset: **Other** — leave build/output settings blank.
4. Click **Deploy**. Vercel gives you a live URL (e.g. `nikithalama-portfolio.vercel.app`) and auto-redeploys on every push to `main`.

**Alternatives:** [GitHub Pages](https://pages.github.com) (Settings → Pages → deploy from `main`) or drag-and-drop the folder into [Netlify](https://app.netlify.com) — both work the same way since there's no build step.

---

## Contact Form

The form in the "Get In Touch" section submits to [Formspree](https://formspree.io) (endpoint already configured in `index.html`). Submission is handled via `fetch` in `script.js`, showing an inline success/error message instead of redirecting the page. Submissions land in the connected Formspree inbox.

## Analytics

`index.html` includes the Vercel Analytics script tag (`/_vercel/insights/script.js`), which activates automatically once deployed on Vercel — view data under the project's **Analytics** tab.

---

## Customization Notes

- **Colors:** edit `tailwind.config.extend.colors.brand` in `index.html` to re-theme the site.
- **Projects:** each project is a `.project-card` block in the `#projects` section — copy one to add another.
- **Pending links:** use a disabled `<button disabled>Coming Soon</button>` and the `.badge-pending` class for projects without a live link.

---

## Contact

- **Email:** nikithalama@gmail.com
- **Phone:** +91 88384 91590
- **LinkedIn:** [linkedin.com/in/nikitha-lama](https://www.linkedin.com/in/nikitha-lama/)
- **GitHub:** [github.com/Nikitha-git266](https://github.com/Nikitha-git266)
