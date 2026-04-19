<div align="center">
  <img src="static/logo.png" alt="Project Logo" width="200">
  <h1>Hugo Recipe Book</h1>
  <p><strong>A modern, high-performance digital recipe book built with Hugo.</strong></p>

  <p>
    <a href="https://github.com/unamatasanatarai/hugo-recipe-book/actions/workflows/hugo.yml"><img src="https://github.com/unamatasanatarai/hugo-recipe-book/actions/workflows/hugo.yml/badge.svg" alt="Deploy Hugo site to Pages"></a>
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT">
    <img src="https://img.shields.io/badge/Tech-Hugo-FF4088?logo=hugo&logoColor=white" alt="Hugo">
    <img src="https://img.shields.io/badge/Language-Polish-white?logo=probot&logoColor=red" alt="Content Language: Polish">
  </p>

  <h4>
    <a href="https://unamatasanatarai.github.io/hugo-recipe-book/">🚀 View Live Project</a>
  </h4>
</div>

---

## 📖 Overview

**Hugo Recipe Vault** is an automated, lightning-fast digital cookbook. Designed for simplicity and performance, it leverages the power of static site generation to provide a seamless reading experience across all devices.

> [!NOTE]  
> While the documentation and repository infrastructure are in **English**, the recipe content itself is written in **Polish**.

## 🛠️ Tech Stack

- **SSG**: [Hugo](https://gohugo.io/) (High-performance Static Site Generator)
- **Content**: Markdown (Structured text for recipes)
- **Automation**: Bash (Custom scripting for Developer Experience)
- **CI/CD**: GitHub Actions (Automated build and deployment)
- **Hosting**: GitHub Pages

## ✨ Key Features

- **Automated Workflow**: A custom `./add` utility script handles recipe creation, filename normalization, and boilerplate generation.
- **Optimized Performance**: Minified production builds with high SEO scores.
- **Search & Filter**: Fast, client-side indexing for recipe discovery.
- **Mobile First**: Responsive design tailored for use in the kitchen.

## 🚀 Getting Started

### Prerequisites

- [Hugo (Extended version)](https://gohugo.io/installation/) installed locally.

### Local Development

1. **Clone the repository**:
   ```bash
   git clone https://github.com/unamatasanatarai/hugo-recipe-book.git
   cd hugo-recipe-book
   ```

2. **Run the development server**:
   ```bash
   hugo server -D
   ```
   Access the site at `http://localhost:1313`.

### Adding a Recipe

We treat content like code. To add a new recipe, use the provided automation tool:

```bash
./add "Nazwa Przepisu"
```
This will:
- Generate a slugified filename.
- Apply the correct Hugo archetype.
- Open the file in your default editor.

## 🤖 CI/CD Pipeline

The project uses GitHub Actions (`.github/workflows/hugo.yml`) to automatically:
1. Lint and build the Hugo site on every push to `main`.
2. Optimize assets (minify HTML/CSS).
3. Deploy the resulting static artifact to GitHub Pages.

## 📂 Project Structure

```text
├── .github/workflows  # CI/CD pipelines
├── content/przepis    # Recipe database (Markdown)
├── layouts/           # Custom Hugo layout overrides
├── static/            # Global assets (logos, etc.)
├── themes/przepisy    # Custom theme logic and styles
├── config.toml        # Site configuration
└── add                # Operations & DX script
```

---

<p align="center">
  Built with 🍫 for better, ad free cooking.
</p>
