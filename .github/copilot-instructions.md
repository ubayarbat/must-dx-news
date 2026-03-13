# AI Coding Agent Instructions for must-dx-news

## Project Overview
This is a Jekyll-based documentation site using the Just the Docs theme, focused on digital culture education content in Mongolian for Mongolian University of Science and Technology (MUST). The site publishes educational articles about digital literacy, ethics, and transformation.

## Architecture
- **Framework**: Jekyll 4.4.1 with just-the-docs theme 0.12.0
- **Content Structure**: 
  - `index.md`: Home page with overview sections
  - `news/`: Directory containing individual article markdown files
  - `_includes/components/`: Custom HTML components (footer.html, sidebar.html)
  - `_includes/`: Theme customizations (search_placeholder_custom.html, toc_heading_custom.html)
- **Build Output**: Generated to `_site/` directory
- **Deployment**: GitHub Pages via Actions workflow

## Key Workflows
- **Local Development**: `bundle exec jekyll serve` (serves at localhost:4000)
- **Build**: `bundle exec jekyll build` (outputs to _site/)
- **Dependencies**: `bundle install` to install gems from Gemfile
- **Preview**: Site builds automatically on push to main branch via .github/workflows/pages.yml

## Content Patterns
- **Language**: All content in Mongolian (Монгол хэл)
- **Front Matter**: Use standard Jekyll front matter with `layout: default`, `title`, `parent`, `nav_order`
- **Navigation**: Articles in `news/` use `parent` to create hierarchical navigation (e.g., `parent: Нэр томьёоны тайлбар`)
- **Examples**:
  ```yaml
  ---
  layout: default
  title: Цахим ба Дижитал
  parent: Нэр томьёоны тайлбар
  nav_order: 1
  ---
  ```

## Customization Conventions
- **Search**: Customized placeholder text in `_includes/search_placeholder_custom.html`
- **Components**: Override theme components in `_includes/components/` (footer, sidebar)
- **Configuration**: Site config in `_config.yml` with Mongolian title, custom footer content, and search settings
- **Assets**: Images stored in `images/` directory, referenced with `/images/` paths

## Development Guidelines
- **Content Creation**: Add new articles as `.md` files in `news/` with appropriate front matter
- **Navigation Updates**: Update `nav_order` and `parent` fields when adding/removing content
- **Theme Customization**: Modify files in `_includes/` to customize Just the Docs appearance
- **Build Validation**: Always run `bundle exec jekyll build` to verify site generates without errors
- **Content Standards**: Maintain educational tone focused on digital literacy and ethics in academic context</content>
<parameter name="filePath">/home/home/src/must-dx-news/.github/copilot-instructions.md