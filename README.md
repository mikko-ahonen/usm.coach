# USM Coach GitHub Pages Site

This directory contains a static Jekyll site for GitHub Pages, converted from the Django public app.

## Structure

```
_config.yml              # Jekyll configuration
_layouts/
└── default.html         # Main layout template
assets/
├── css/
│   └── style.css        # Minimal CSS styling
│   ├── img/                 # Images from Django static files
│   └── pdf/                 # PDF resources
about/
└── index.html           # About page
services/
└── index.html           # Services page
resources/
└── index.html           # Resources page
contact/
└── index.html           # Contact page
privacy-policy/
└── index.html           # Privacy policy page
index.html               # Home page (redirects to about)
```

## Setup for GitHub Pages

1. Go to your repository settings on GitHub
2. Navigate to Pages section
3. Under "Source", select "Deploy from a branch"
4. Select the `master` branch and `/docs` folder
5. Click Save

Your site will be available at: `https://<username>.github.io/<repository>/`

## Local Testing

To test locally with Jekyll:

```bash
cd docs
bundle exec jekyll serve
```

Then visit `http://localhost:4000`

## Notes

- All Django template translations have been converted to static English content
- The resources page form functionality has been removed (static site)
- All internal links use Jekyll's `relative_url` filter for proper path handling
- The site uses a minimal, responsive CSS design
