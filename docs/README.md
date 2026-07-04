# Hugo Site for GitHub Pages

This is a Hugo static site generator configured for GitHub Pages.

## Local Development

### Prerequisites
- Install [Hugo](https://gohugo.io/installation/) (extended version recommended)

### Running Locally

```bash
cd docs
hugo server
```

The site will be available at `http://localhost:1313`

## Building

```bash
cd docs
hugo
```

This creates the static site in the `docs/public` folder.

## Deployment

The site is automatically deployed to GitHub Pages when you push to the main branch using the GitHub Actions workflow (`.github/workflows/hugo.yml`).

## Project Structure

```
docs/
├── hugo.toml          # Hugo configuration
├── content/           # Site content (markdown files)
│   ├── _index.md      # Home page
│   └── posts/         # Blog posts directory
├── layouts/           # Custom layouts (optional)
├── static/            # Static files (images, CSS, etc.)
├── themes/            # Hugo themes
└── public/            # Built site (generated)
```

## Adding Themes

To add a theme, you can either clone it into the `themes` directory or add it as a git submodule:

```bash
cd docs
git submodule add https://github.com/theNewDynamic/ananke.git themes/ananke
```

Then update `hugo.toml` to set the theme.

## More Information

- [Hugo Documentation](https://gohugo.io/documentation/)
- [GitHub Pages Setup](https://docs.github.com/en/pages)