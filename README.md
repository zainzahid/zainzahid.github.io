# Zain Zahid's Portfolio Website

[![Deploy Hugo site to Pages](https://github.com/zainzahid/zainzahid.github.io/actions/workflows/hugo.yml/badge.svg)](https://github.com/zainzahid/zainzahid.github.io/actions/workflows/hugo.yml)

Personal portfolio website built with [Hugo](https://gohugo.io/) - a fast and modern static site generator.

🌐 **Live Site:** [https://zainzahid.github.io](https://zainzahid.github.io)

## About

This is the personal portfolio website of Zain Zahid, a Full Stack AI Engineer with over 7 years of experience in diverse work environments. The site showcases experience, skills, education, awards, and certifications.

## Tech Stack

- **Static Site Generator:** Hugo v0.150.0+
- **Theme:** Custom portfolio theme
- **Deployment:** GitHub Pages with GitHub Actions
- **Styling:** Custom CSS with Bootstrap 5.1.3 integration
- **Icons:** Bootstrap Icons, Boxicons
- **Fonts:** Space Grotesk, Google Fonts

## Development

### Prerequisites

- [Hugo](https://gohugo.io/installation/) v0.150.0 or later (extended version)

### Local Development

```bash
# Start development server
npm run dev
# or
hugo server --buildDrafts --buildFuture

# Build for production
npm run build
# or
hugo --gc --minify

# Preview production build
npm run preview

# Clean build artifacts
npm run clean
```

The development server will be available at `http://localhost:1313`

## Project Structure

```
├── content/           # Markdown content files
│   ├── awards/        # Awards section
│   ├── certifications/# Certifications section
│   ├── education/     # Education section
│   ├── experience/    # Experience section
│   └── skills/        # Skills section
├── themes/portfolio/  # Custom Hugo theme
│   ├── layouts/       # Template files
│   └── static/        # Static assets
├── static/           # Global static files
│   └── assets/       # Images, fonts, etc.
├── .github/workflows/# GitHub Actions
└── hugo.toml         # Hugo configuration
```

## Content Management

Content is managed through Markdown files in the `content/` directory. Each section has its own `_index.md` file:

- **Experience:** `/content/experience/_index.md`
- **Skills:** `/content/skills/_index.md`
- **Education:** `/content/education/_index.md`
- **Awards:** `/content/awards/_index.md`
- **Certifications:** `/content/certifications/_index.md`

## Deployment

The site is automatically deployed to GitHub Pages using GitHub Actions when changes are pushed to the `master` branch. The workflow is defined in `.github/workflows/hugo.yml`.



