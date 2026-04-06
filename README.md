# Portfolio — Vaibhav

A minimal, responsive HTML/CSS portfolio website showcasing projects and skills in cloud infrastructure and web development.

## Features

- **Responsive Design** — Works beautifully on desktop, tablet, and mobile devices
- **Fast & Lightweight** — Pure HTML & CSS, no JavaScript dependencies
- **Dark Theme** — Modern, eye-friendly dark mode aesthetic
- **Accessible** — Semantic HTML and ARIA labels for screen readers

## Project Structure

```
.
├── index.html          # Main portfolio page
├── css/
│   └── styles.css      # Styling and responsive layout
├── .gitignore          # Git ignore rules
└── README.md           # This file
```

## Quick Start

### View Locally

Option 1: Open directly in your browser
```bash
open index.html
```

Option 2: Serve with a local HTTP server (recommended)
```bash
python3 -m http.server 8000
# Then open http://localhost:8000
```

## Customization

Edit `index.html` to update:
- Your name and headline in the hero section
- About section text
- Project cards (title, description, links, tags)
- Contact information (email, location)

Edit `css/styles.css` to customize:
- Color scheme (CSS variables at the top: `--bg`, `--card`, `--accent`, etc.)
- Typography and spacing
- Animations and transitions

## Deployment

### GitHub Pages

```bash
git push origin main
```

Then go to your repository settings and enable GitHub Pages with the `main` branch.

### AWS S3 + CloudFront

```bash
aws s3 sync . s3://your-bucket-name --exclude ".git*"
# Create CloudFront distribution pointing to your S3 bucket
```

### Other Platforms

Works with Netlify, Vercel, or any static hosting service. Simply point to this directory or push to their Git integration.

## Technologies

- HTML5
- CSS3 (Grid, Flexbox, CSS Variables)
- No frameworks or build tools required

## License

Open source — feel free to fork and modify for your own portfolio.
