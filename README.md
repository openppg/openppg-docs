# OpenPPG Documentation

Official documentation website for OpenPPG electric paramotors, including the SP140 v2.5 User Manual, guides, and technical resources.

🌐 **Live Site:** [docs.openppg.com](https://docs.openppg.com)

## About

This repository contains the complete documentation for OpenPPG products, built with [Hugo](https://gohugo.io/) and the [Doks theme](https://getdoks.org/). The site provides comprehensive guides for assembly, operation, maintenance, and troubleshooting of OpenPPG electric paramotors.

## Features

- **SP140 v2.5 User Manual** - Complete assembly and operation guide
- **Technical Specifications** - Performance data and specifications
- **Video Tutorials** - Step-by-step assembly and flight guides
- **Community Resources** - Links to forums and support

## Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) v0.154.5 or later
- [Node.js](https://nodejs.org/) v20.11.0 or later
- [npm](https://www.npmjs.com/) v10 or later

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/openppg/openppg-docs.git
   cd openppg-docs
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Verify Hugo installation:**
   ```bash
   hugo version
   ```
   Make sure you have Hugo Extended version 0.154.5 or later.

## Local Development

**Start the development server:**
```bash
npm run dev
```

This will start Hugo's development server with live reload at `http://localhost:1313/`

**Other useful commands:**
```bash
# Create new content
npm run create content/docs/new-page.md

# Build for production
npm run build

# Preview production build
npm run preview

# Format code
npm run format
```

## Project Structure

```
openppg-docs/
├── assets/              # Images, JS, SCSS
├── config/              # Hugo configuration
│   └── _default/        # Main config files
├── content/             # Markdown content
│   └── docs/            # Documentation pages
│       └── sp140-manual/  # SP140 v2.5 manual
├── layouts/             # Custom Hugo templates
├── static/              # Static assets
└── package.json         # Node dependencies
```

## Contributing

We welcome contributions to improve the documentation! Here's how you can help:

### Reporting Issues

- Found a typo or error? [Open an issue](https://github.com/openppg/openppg-docs/issues)
- Include the page URL and a description of the problem

### Submitting Changes

1. **Fork the repository**
2. **Create a feature branch:**
   ```bash
   git checkout -b improve-assembly-guide
   ```
3. **Make your changes** - Edit Markdown files in `content/docs/`
4. **Test locally:**
   ```bash
   npm run dev
   ```

5. **Format your code:**
   ```bash
   npm run format
   ```
6. **Commit your changes:**
   ```bash
   git commit -am "Improve assembly step 3 clarity"
   ```
6. **Push to your fork:**
   ```bash
   git push origin improve-assembly-guide
   ```
7. **Create a Pull Request**

### Content Guidelines

- Use clear, concise language
- Follow the existing formatting style
- Include images when helpful (place in `/content/docs/[section]/images/`)
- Test all links and references
- Ensure proper front matter in Markdown files

## Deployment

The site automatically deploys to GitHub Pages when changes are pushed to the `master` branch. The deployment workflow:

1. Installs Hugo v0.154.x
2. Installs npm dependencies
3. Builds the site with `hugo --minify`
4. Deploys to GitHub Pages

See [.github/workflows/deploy.yml](.github/workflows/deploy.yml) for details.

## Technology Stack

- **[Hugo](https://gohugo.io/)** - Static site generator
- **[Doks](https://getdoks.org/)** - Hugo documentation theme
- **[Thulite](https://thulite.io/)** - Component library
- **[Tabler Icons](https://tablericons.com/)** - Icon set

## Support

- **Documentation Issues:** [GitHub Issues](https://github.com/openppg/openppg-docs/issues)
- **Community Forum:** [community.openppg.com](https://community.openppg.com)
- **Website:** [openppg.com](https://openppg.com)
