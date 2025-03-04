# My Hugo Blog

This repository contains the source code for my personal blog built with [Hugo](https://gohugo.io/), a fast and modern static site generator.

## Overview

This blog is built using Hugo and hosted on GitHub Pages.

## Prerequisites

To work with this repository, you'll need:

- [Hugo](https://gohugo.io/getting-started/installing/) (Extended version recommended)
- [Git](https://git-scm.com/downloads)
- A code editor of your choice (Nvim, VS Code, etc.)

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
```

### Run the Development Server

```bash
hugo server -D
```

This will start a local development server at `http://localhost:1313/` with live reloading enabled.

## Project Structure

```
.
├── archetypes/        # Template files for new content
├── assets/            # Unprocessed assets like SCSS or JS
├── content/           # Markdown files containing site content
├── data/              # Configuration files for the site
├── layouts/           # Templates for converting content into HTML
├── static/            # Static files like images, CSS, JS
├── themes/            # Site themes
├── config.toml        # Site configuration
└── README.md          # This file
```

## Creating New Content

To create a new blog post:

```bash
hugo new posts/my-new-post.md
```

Then edit the newly created file in the `content/posts/` directory.

## Deployment

This site is deployed using [GitHub Actions/GitHub Pages/Netlify/etc.]. When changes are pushed to the main branch, the site is automatically built and deployed.


## Customization

### Theme

This blog uses the [m10c](https://themes.gohugo.io/themes/hugo-theme-m10c/) theme, a minimalistic and responsive theme for Hugo.

#### Installing the Theme

If you're setting up the repository from scratch, you can install the theme with:

```bash
git clone https://github.com/vaga/hugo-theme-m10c.git themes/hugo-theme-m10c
```

Then add this line to your `config.toml` file:

```toml
theme = "hugo-theme-m10c"
```

#### Theme Configuration

The m10c theme can be customized through the `config.toml` file. Here are the main configuration options:

```toml
[params]
  author = "Your Name"
  description = "Your description here"
  menu_item_separator = " - "
  
  # Avatar/profile picture (place in static/images/)
  avatar = "/images/your-avatar.jpg"
  
  # Social media links
  [[params.social]]
    icon = "github"
    name = "GitHub"
    url = "https://github.com/yourusername"
  
  [[params.social]]
    icon = "twitter"
    name = "Twitter"
    url = "https://twitter.com/yourusername"
  
  # You can add more social links following the same pattern
  
  # Custom theme colors
  [params.style]
    darkestColor = "#242930"
    darkColor = "#353b43"
    lightColor = "#afbac4"
    lightestColor = "#ffffff"
    primaryColor = "#57cc8a"
```

Available social icons include: `email`, `facebook`, `github`, `gitlab`, `instagram`, `linkedin`, `stackoverflow`, `telegram`, `twitter`, `youtube`, and more.

### Configuration

The main configuration file is `config.toml`. Edit this file to change site title, base URL, language settings, and other global configurations.

## Contributing

If you'd like to contribute to this blog:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some feature'`)
5. Push to the branch (`git push origin feature/your-feature`)
6. Open a Pull Request


## Acknowledgments

- Hugo team for the amazing static site generator
- [vaga](https://github.com/vaga) for the [m10c](https://github.com/vaga/hugo-theme-m10c) theme
