# Instructor Setup Guide

This guide helps instructors set up and customize the student portfolio template for their specific course needs.

## Quick Setup for Instructors

### 1. Template Customization

Before sharing with students, customize these files:

#### `_quarto.yml`
- Update the default title: Change "Your Name - Data Science Portfolio" to match your course
- Modify navigation structure based on your course projects
- Adjust the theme if desired (options: cosmo, flatly, darkly, etc.)

#### `README.md`
- Update course-specific information
- Modify project categories to match your curriculum
- Add your institution's specific requirements

### 2. Creating Course-Specific Versions

#### Option A: GitHub Template Repository
1. Create a new repository from this template
2. Customize for your course
3. Students can use "Use this template" button

#### Option B: Fork and Customize
1. Fork this repository
2. Make course-specific changes
3. Share the fork link with students

### 3. Student Instructions Template

Copy and customize this text for your course:

```markdown
## Course-Specific Setup

1. Use this template repository to create your portfolio
2. Replace "Your Name" with your actual name in all files
3. Update the GitHub and LinkedIn links in `_quarto.yml`
4. Follow the project structure for Assignment X, Y, Z...

## Required Projects for [Course Name]

- [ ] Assignment 1: Exploratory Data Analysis
- [ ] Assignment 2: Data Acquisition Project  
- [ ] Assignment 3: Statistical Analysis
- [ ] Final Project: [Specific requirements]

## Submission Guidelines

- Deploy your site to GitHub Pages
- Submit the repository URL and live site URL
- Ensure all code runs without errors
- Include proper documentation and citations
```

### 4. Grading Rubric Suggestions

#### Technical Implementation (40%)
- [ ] Site builds and deploys successfully
- [ ] Code runs without errors
- [ ] Proper use of Quarto features (code folding, citations, etc.)
- [ ] Professional site navigation and structure

#### Content Quality (40%)
- [ ] Clear project descriptions and methodology
- [ ] Appropriate data visualization and analysis
- [ ] Well-documented code with comments
- [ ] Professional writing and presentation

#### Portfolio Presentation (20%)
- [ ] Consistent formatting and style
- [ ] Effective use of visual elements
- [ ] Professional About page and contact information
- [ ] Demonstrates learning progression

### 5. Common Student Issues and Solutions

#### Issue: "Quarto won't render"
**Solution**: Check for:
- Python/R installation issues
- Missing packages (create requirements.txt)
- YAML syntax errors in frontmatter

#### Issue: "GitHub Pages not updating"
**Solution**: 
- Ensure GitHub Pages is enabled
- Check that output-dir is set to "docs"
- Verify the main branch has the docs folder

#### Issue: "Code doesn't run"
**Solution**:
- Provide a template environment.yml or requirements.txt
- Include setup instructions for common packages
- Consider using Binder or Google Colab links

### 6. Customization Options

#### For Programming-Heavy Courses
Add to `_quarto.yml`:
```yaml
format:
  html:
    code-link: true
    code-copy: true
    code-overflow: wrap
```

#### For Research-Focused Courses
Add bibliography support:
```yaml
bibliography: references.bib
csl: apa.csl
```

#### For Collaborative Projects
Consider adding:
- Team member attribution sections
- Shared data folders
- Collaboration guidelines

### 7. Assessment Integration

#### Portfolio Checkpoints
Suggested timeline:
- Week 3: Site setup and About page
- Week 6: First project completed
- Week 10: Mid-semester portfolio review
- Week 15: Final portfolio submission

#### Peer Review Activities
- Portfolio gallery walks
- Peer feedback sessions
- Cross-project citations and references

### 8. Advanced Features

#### Analytics (Optional)
Add Google Analytics to `_quarto.yml`:
```yaml
website:
  google-analytics: "G-XXXXXXXXXX"
```

#### Comments (Optional)
Enable utterances for commenting:
```yaml
comments:
  utterances:
    repo: username/repo-name
```

### 9. Maintenance Tips

#### Keep Template Updated
- Regularly update package versions
- Monitor Quarto updates for new features
- Collect student feedback for improvements

#### Backup Strategy
- Encourage students to commit regularly
- Provide Git best practices guide
- Consider automated backup solutions

### 10. Troubleshooting Resources

Create a course FAQ with:
- Common error messages and solutions
- Links to Quarto documentation
- Office hours schedule for technical help
- Student collaboration guidelines

## Additional Resources for Instructors

- [Quarto for Academics](https://quarto.org/docs/blog/posts/2022-10-25-jupyter-authoring/)
- [GitHub Classroom Integration](https://classroom.github.com/)
- [Teaching with GitHub Pages](https://docs.github.com/en/education)

## Support

For technical issues with this template:
- Check the [Quarto documentation](https://quarto.org/docs/)
- Review GitHub Issues in this repository
- Contact [your support information]

---

*This template is designed to be flexible and adaptable to various data science course structures.*
