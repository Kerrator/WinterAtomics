# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based academic portfolio website for GitHub Pages deployment. The site uses a minimal, content-focused design with Tufte CSS for academic styling.

## Development Commands

### Local Development
```bash
# Install Jekyll and dependencies (if not already installed)
gem install jekyll bundler

# Serve the site locally
jekyll serve

# Serve with drafts
jekyll serve --drafts

# Build the site
jekyll build
```

The site will be available at `http://localhost:4000` when running locally.

### GitHub Pages Deployment
No build commands needed - GitHub Pages automatically builds Jekyll sites when pushed to the repository. Ensure the repository settings have GitHub Pages enabled with source set to the main branch.

## Architecture

### Site Structure
- **[_config.yml](_config.yml)**: Jekyll configuration including site metadata (title, description, author, contact info), collections, and plugins
- **[_layouts/default.html](_layouts/default.html)**: Layout template with CSS Grid sidebar navigation, Tufte CSS, and custom academic styling
- **[_data/](_data/)**: YAML data files for dynamic content
  - **[publications.yml](_data/publications.yml)**: Research publications with graphical abstracts
- **[assets/images/](assets/images/)**: Directory for graphical abstracts and other images
- **Pages**:
  - **[index.md](index.md)**: Homepage with bio
  - **[research.md](research.md)**: Research overview and methods
  - **[teaching.md](teaching.md)**: Teaching philosophy and interests
  - **[publications.md](publications.md)**: Publications list with graphical abstracts

### Design System
- Uses Tufte CSS (CDN-loaded) for academic, readable typography
- CSS Grid layout with sidebar navigation (250px sidebar + main content)
- Responsive design: sidebar collapses to horizontal navigation on mobile (< 768px)
- Custom styles in [default.html](_layouts/default.html#L16-L260)
- Max-width 1200px for entire site, 800px for main content
- Palatino/Georgia serif font stack for academic aesthetic
- Sidebar includes navigation links and contact information

### Collections Configuration
The site defines `publications` and `videos` collections in [_config.yml](_config.yml), but uses data file approach for publications ([_data/publications.yml](_data/publications.yml)).

## Content Management

### Adding Publications
Edit [_data/publications.yml](_data/publications.yml) following the format:
```yaml
- title: "Paper Title"
  authors: "Author 1, Author 2, Author 3"
  year: 2024
  venue: "Conference or Journal Name"
  link: "https://example.com/paper-link"
  image: "/assets/images/pub-2024-example.png"
  type: "journal"  # Options: journal, conference, preprint, poster, talk
```

**Adding graphical abstracts:**
1. Save publication images to [assets/images/](assets/images/) directory
2. Reference them in the `image` field with path `/assets/images/filename.png`
3. Recommended image size: max 400px wide for optimal performance
4. Images display on the [publications.md](publications.md) page

### Updating Site Content
- **Site metadata**: Edit [_config.yml](_config.yml) to modify title, description, author, email, LinkedIn
- **Bio**: Edit [index.md](index.md)
- **Research content**: Edit [research.md](research.md)
- **Teaching content**: Edit [teaching.md](teaching.md)
- **Navigation**: Modify sidebar navigation in [_layouts/default.html](_layouts/default.html#L270-L286)

## Key Technical Details

- **Markdown processor**: kramdown (configured in [_config.yml](_config.yml#L7))
- **SEO**: Uses `jekyll-seo-tag` plugin ([_config.yml](_config.yml#L15-L16))
- **Theme**: Custom theme (no gem-based theme) with all styling in layout file
- **Default layout**: All pages use `default` layout unless specified ([_config.yml](_config.yml#L26-L30))
