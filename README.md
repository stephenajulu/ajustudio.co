# AJU studio (`ajustudio.co`)

> Bespoke branding and design studio based in Nairobi, Kenya. Crafting distinctive visual identities, digital experiences, and design systems in the pursuit of impact and excellence.

---

## ⚡ Tech Stack & Architecture

* **Engine**: [GoHugo](https://gohugo.io/) (v0.160.1+ Extended)
* **CMS**: [CloudCannon](https://cloudcannon.com/) (first-class Git-based visual editor & page builder)
* **Styling**: SCSS via Hugo Pipes (`css.Sass`), modular BEM structure with palette variations
* **Asset Pipeline**: Automated SCSS transpilation, CSS minification, and cache-busting via fingerprinting with Subresource Integrity (SRI)
* **Metadata & SEO**: Centralized Open Graph, Twitter Cards, canonical links, and Schema.org JSON-LD structured data (`ProfessionalService`, `BlogPosting`, `CreativeWork`)
* **Deployment**: [Netlify](https://www.netlify.com/) (`netlify.toml`), CloudCannon, & [GitHub Actions](https://github.com/features/actions) (`.github/workflows/ci.yml`)

---

## 📁 Project Structure

```text
├── assets/
│   └── sass/              # Modular SCSS stylesheets & palette tokens
├── content/
│   ├── _index.md          # Homepage (component slices)
│   ├── about.md           # About / Studio story
│   ├── contact.md         # Inquiries & project contact form
│   ├── thank-you.md       # Form submission confirmation
│   ├── blog/              # Journal & insights
│   └── portfolio/         # Studio projects & case studies
├── data/
│   └── config.json        # Global studio configuration, navigation & social profiles
├── layouts/
│   ├── _default/          # Base template (baseof.html), section & page layouts
│   └── partials/          # Reusable component slices (hero, portfolio, grid, cta, seo)
├── static/                # Static assets, SVG logos, photography
├── config.yaml            # Hugo site configuration
└── netlify.toml           # Netlify build configuration
```

---

## 🚀 Local Development

### Prerequisites

Ensure you have **Hugo Extended** (v0.160.0 or higher) installed:

```bash
hugo version
# Example: hugo v0.160.1+extended ...
```

### Running the Dev Server

Start the Hugo development server with live reload:

```bash
hugo server -D
```

Open [http://localhost:1313/](http://localhost:1313/) in your browser.

### Building for Production

Compile minified production assets into the `public/` directory:

```bash
hugo --gc --minify
```

---

## 🛠️ Configuration & Content Management

* **CloudCannon CMS**: Log into [CloudCannon](https://cloudcannon.com/) and connect this repository. CloudCannon will automatically detect [`cloudcannon.config.yaml`](file:///C:/Users/ajulu/Desktop/PROJECTS/Dev%20PROJECTS/ajustudio.co/cloudcannon.config.yaml), enabling visual inline editing, component block reordering (hero, services, portfolio, forms, CTA), and live previews.
* **Site Settings & Navigation**: Edit [`data/config.json`](file:///C:/Users/ajulu/Desktop/PROJECTS/Dev%20PROJECTS/ajustudio.co/data/config.json) to update header links, studio details, brand palette, and social URLs.
* **Homepage Slices**: Edit [`content/_index.md`](file:///C:/Users/ajulu/Desktop/PROJECTS/Dev%20PROJECTS/ajustudio.co/content/_index.md) to add, remove, or reorder homepage sections (`hero_section`, `portfolio_section`, `grid_section`, `cta_section`).
* **Portfolio Items**: Add new project Markdown files inside [`content/portfolio/`](file:///C:/Users/ajulu/Desktop/PROJECTS/Dev%20PROJECTS/ajustudio.co/content/portfolio/) (or click *Add New Project* in CloudCannon).
* **Journal Entries**: Add new articles inside [`content/blog/`](file:///C:/Users/ajulu/Desktop/PROJECTS/Dev%20PROJECTS/ajustudio.co/content/blog/) (or click *Add New Article* in CloudCannon).

---

## 📄 License & Credits

© AJU studio. All rights reserved.
