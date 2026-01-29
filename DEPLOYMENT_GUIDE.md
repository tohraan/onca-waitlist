# ONCA Deployment Guide

This folder contains the production-ready build for the ONCA landing page, including the high-end scroll-driven animation.

## What's Inside
- `index.html`: The main entry point.
- `assets/`: Optimized CSS and JavaScript bundles.
- `frames/`: Preloaded video frames for the hero animation.

## How to Deploy

### Option 1: Static Hosting (Recommended)
You can upload the contents of this folder directly to any static hosting provider:
- **Vercel**: Run `vercel` in this directory or connect your GitHub repo.
- **Netlify**: Drag and drop this folder onto the Netlify dashboard.
- **GitHub Pages**: Push the contents of this folder to a `gh-pages` branch.
- **AWS S3 / CloudFront**: Upload the files to an S3 bucket configured for website hosting.

### Option 2: Local Preview
If you want to preview the deployment build locally, you can use a simple static server.

#### Using Node.js (npx)
```bash
npx serve
```

#### Using Python
```bash
python3 -m http.server 8000
```

## Notes
- Ensure that the `frames/` directory is served correctly, as the animation relies on these assets being available at `/frames/ezgif-frame-XXX.jpg`.
- The build uses modern JavaScript and CSS. It's optimized for performance and includes preloading for the hero animation assets.
