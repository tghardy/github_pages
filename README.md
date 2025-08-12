# Student Portfolio Template

This repository provides a template for creating a personal data science portfolio website using [Quarto](https://quarto.org/) and [GitHub Pages](https://pages.github.com/). Students will use this template to showcase their projects and learning journey throughout the course.

## 🚀 Getting Started

### Prerequisites
- [Quarto](https://quarto.org/docs/get-started/) installed on your computer
- A GitHub account
- Basic knowledge of Markdown

### Setup Instructions

1. **Create your repository**
   - Click "Use this template" button (or fork this repository)
   - Name your repository `your-username.github.io` for a personal site, or any name you prefer
   - Make sure it's set to **Public**

2. **Clone your repository**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

3. **Customize your site**
   - Edit `_quarto.yml` to update the site title and navigation
   - Modify `index.md` to create your homepage
   - Add your projects as `.qmd` or `.md` files

4. **Build and preview locally**
   ```bash
   quarto preview
   ```

5. **Deploy to GitHub Pages**
   - Build your site: `quarto render`
   - Commit and push your changes
   - Enable GitHub Pages in your repository settings (Settings → Pages → Source: Deploy from a branch → Branch: main → Folder: /docs)

## 📁 Repository Structure

```
├── _quarto.yml          # Site configuration
├── index.md             # Homepage
├── README.md            # This file
├── docs/                # Generated site files (auto-created)
├── projects/            # Your project files
│   └── example.qmd      # Example project file
└── assets/              # Images, data files, etc.
```

## 📝 Adding Content

### Creating a New Project Page

1. Create a new `.qmd` file in the `projects/` folder
2. Add YAML frontmatter at the top:
   ```yaml
   ---
   title: "Your Project Title"
   author: "Your Name"
   date: "2024-01-01"
   format:
     html:
       code-fold: true
       toc: true
   ---
   ```
3. Add your content using Markdown and code chunks
4. Update `_quarto.yml` to include the new page in navigation

### Supported Content Types

- **Markdown text** with standard formatting
- **Code chunks** in Python, R, Julia, and more
- **Mathematical equations** using LaTeX syntax
- **Interactive plots** and visualizations
- **Images and media** files

## 🎯 Portfolio Sections (Suggested)

Customize these sections based on your course requirements:

### Core Pages
- **About Me** - Personal introduction and background
- **Projects Overview** - Summary of all your work
- **Resume/CV** - Professional experience and skills

### Project Categories
- **Exploratory Data Analysis (EDA)** - Data investigation and visualization projects
- **Data Acquisition & Cleaning** - Web scraping, APIs, data wrangling
- **Statistical Analysis** - Hypothesis testing, modeling projects
- **Machine Learning** - Predictive modeling and classification projects
- **Final Project** - Capstone or comprehensive project

### Additional Sections
- **Blog Posts** - Reflections on learning, tutorials you've written
- **Resources** - Useful links, datasets, tools you've discovered
- **Contact** - How to reach you professionally

## 🛠️ Customization Tips

### Styling Your Site
- Modify the `theme` in `_quarto.yml` to change the appearance
- Add custom CSS by creating a `styles.css` file
- Include your own logo or favicon

### Navigation
- Update the `navbar` section in `_quarto.yml` to add/remove pages
- Create dropdown menus for organized navigation
- Add external links to your GitHub, LinkedIn, etc.

### Code Presentation
- Use `code-fold: true` to make code collapsible
- Add `code-tools: true` for interactive code viewing
- Include `fig-cap` for proper figure captions

## 📚 Resources

- [Quarto Documentation](https://quarto.org/docs/)
- [Quarto Gallery](https://quarto.org/docs/gallery/) - Examples and inspiration
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)

## 🆘 Troubleshooting

### Common Issues
- **Site not updating**: Check that GitHub Pages is enabled and pointing to the `/docs` folder
- **Build errors**: Run `quarto check` to diagnose issues
- **Local preview not working**: Ensure Quarto is properly installed and updated

### Getting Help
- Check the [Quarto FAQ](https://quarto.org/docs/faq/)
- Post questions in course discussion forums
- Review classmates' repositories for examples

## 📄 License

This template is provided for educational purposes. Feel free to modify and use it for your personal portfolio.

---

**Happy coding and showcasing your data science journey! 🎉**

