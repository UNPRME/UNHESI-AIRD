# Design System Demo

A scaffolded static site built with **Jekyll** and a simple design system. The project showcases:

1. Shared CSS variables and component styles located in `assets/css/style.css`.
2. Template inheritance using Jekyll layouts (`_layouts/`).
3. Content managed through a custom collection (`_cards/`) and rendered as cards on the home page.

## Getting Started Locally

1. Install Ruby & Bundler (if you don't already have them):

   ```bash
   gem install bundler jekyll
   ```

2. Serve the site locally:

   ```bash
   bundle install
   bundle exec jekyll serve
   ```

3. Visit <http://localhost:4000> to view.

## Deploying on GitHub Pages

Push this repository to GitHub and enable **GitHub Pages** in the repository settings. Choose the **GitHub Actions** or **Pages** source that suits you (e.g. `main` branch). GitHub will build the site with Jekyll automatically.

## Customisation

- Update the design tokens in `assets/css/style.css` to tweak colours, fonts, spacing, etc.
- Add or edit cards by creating markdown files in `/_cards/` with front-matter fields:

  ```yaml
  ---
  layout: card
  title: "My Card"
  description: "Short summary shown on the grid."
  image: "https://example.com/cover.jpg"
  ---
  
  Content of the page…
  ```
