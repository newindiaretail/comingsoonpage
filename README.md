# New India Retail - Landing Page

A modern, responsive static landing page for New India Retail - reimagining retail for the new aspiring India.

## Overview

New India Retail is a platform dedicated to making every rupee work harder for value and quality-conscious consumers in India. This landing page serves as the company's public face, allowing visitors to learn about our mission and join the waitlist.

## Features

- Modern, clean design with smooth animations
- Fully responsive (mobile, tablet, desktop)
- Fast loading (no external dependencies except Google Fonts)
- SEO-friendly meta tags
- Accessible design
- Email waitlist signup form

## Deployment to GitHub Pages

### Option 1: Deploy from main branch

1. Create a new repository on GitHub named `new-india-retail` (or your preferred name)

2. Initialize and push the code:
   ```bash
   cd new-india-retail
   git init
   git add .
   git commit -m "Initial commit: New India Retail landing page"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/new-india-retail.git
   git push -u origin main
   ```

3. Go to your repository on GitHub → Settings → Pages

4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`

5. Click Save. Your site will be live at `https://YOUR_USERNAME.github.io/new-india-retail/`

### Option 2: Use a custom domain

1. Complete Option 1 first

2. In your domain registrar, add a CNAME record:
   - Name: `www` (or your subdomain)
   - Value: `YOUR_USERNAME.github.io`

3. Create a `CNAME` file in your repository with your domain:
   ```
   www.newindiaretail.in
   ```

4. In GitHub Pages settings, enter your custom domain

## Local Development

Simply open `index.html` in your browser. No build tools required.

For live reload during development, you can use:
```bash
npx serve .
```

## Structure

```
new-india-retail/
├── index.html      # Main landing page (HTML, CSS, JS all-in-one)
├── README.md       # This file
└── CNAME           # Custom domain (create if needed)
```

## Customization

### Colors
The color scheme is defined in CSS variables at the top of `index.html`:
- `--primary`: Dark blue (`#1a1a2e`)
- `--accent`: Coral red (`#e94560`)
- `--gold`: Warm orange (`#f4a261`)
- `--sage`: Teal green (`#2a9d8f`)

### Content
All content is in `index.html`. Key sections:
- Hero section with main headline
- Value propositions grid
- Promise section
- How it works steps
- Waitlist signup form

### Waitlist Form
The form currently shows an alert on submission. To connect to a backend:
1. Replace the form handler in the `<script>` section
2. Options: Google Forms, Airtable, Mailchimp, custom API

## License

Copyright 2026 New India Retail. All rights reserved.
