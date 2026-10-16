<div align="center">
  <img src="images/logo.png" alt="Wedgeworth Plumbing" width="200">
  <h1>Wedgeworth Plumbing</h1>
  <p>A responsive website for Houston plumbing services.</p>
</div>

## About

Wedgeworth Plumbing is a single-page website for a Houston plumbing company. It brings emergency contact options, service information, coverage details, customer reviews, homeowner guides, and a service request form together in one place.

## Highlights

- Responsive layouts for mobile, tablet, and desktop
- Prominent click-to-call emergency contact links
- Service request form with an on-page confirmation state
- Service, coverage, reviews, and homeowner guide sections
- Scroll-triggered reveals and subtle hover effects
- Reduced-motion support for visitors who prefer less animation

## Run locally

### Requirements

- Node.js and npm

### Start the site

```bash
npm install
npm start
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

The site is static HTML and does not require a build step. The service request form currently displays a confirmation in the browser; it is not connected to a dispatch system or backend.

## Deploy to Vercel

1. Push this project to a GitHub repository.
2. In Vercel, choose **Add New → Project** and import the repository.
3. Keep the project root as `.` and select **Other** as the framework preset.
4. Leave the build command and output directory blank; this site is served directly from its root and has no production build step.
5. Deploy. Vercel will create preview deployments for subsequent GitHub changes and production deployments from the configured production branch.

No environment variables are required. The page uses Tailwind CSS from its CDN, so the deployed site needs network access to that CDN and to Google Fonts. The request form is front-end only and does not send submissions to the business.

## Built with

- HTML
- Tailwind CSS via its CDN
- Vanilla JavaScript
- Plus Jakarta Sans and Material Symbols

## Project structure

```text
.
├── index.html          # Website
├── images/             # Logo and image assets
├── .gitignore          # Local dependencies, Vercel files, and environment files
├── DESIGN.md           # Design system notes
├── design-system.json  # Color and typography tokens
├── site-manifest.json  # Site screen and asset metadata
├── package.json        # Local preview scripts and dependencies
└── README.md
```

## Design

The visual style pairs deep greens and warm gold accents with clean, high-contrast layouts. See [DESIGN.md](DESIGN.md) and [design-system.json](design-system.json) for the design guidelines and tokens.
