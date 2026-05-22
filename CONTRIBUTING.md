# Contributing Guidelines

Thank you for your interest in contributing to the Preliminaries of Web repository! This document provides guidelines for making meaningful contributions to this educational project.

---

## 🤝 Ways to Contribute

### 1. Report Issues
- Found an error in the HTML/CSS?
- Documentation unclear or incorrect?
- Broken links or resources?
- **Open an issue** on GitHub with:
  - Clear title and description
  - Steps to reproduce (if applicable)
  - Expected vs. actual behavior
  - Screenshots or code examples

### 2. Improve Documentation
- Clarify existing documentation
- Add examples or explanations
- Fix typos or grammatical errors
- Enhance learning resources

### 3. Enhance Learning Materials
- Add new activities or exercises
- Create additional examples
- Develop practice projects
- Add learning assessments

### 4. Fix Bugs or Issues
- Correct HTML errors
- Fix CSS issues
- Improve code structure
- Optimize for accessibility

### 5. Share Resources
- Contribute relevant learning links
- Share useful tutorials
- Add best practice guides
- Recommend tools

---

## 📋 Getting Started

### Prerequisites
- Familiarity with Git and GitHub
- Understanding of HTML and CSS basics
- Knowledge of this project's scope
- Read all documentation files first

### Setup Your Environment
```bash
# 1. Fork the repository
# Click "Fork" on GitHub

# 2. Clone your fork
git clone https://github.com/YOUR_USERNAME/Preliminaries-of-web.git

# 3. Navigate to the directory
cd Preliminaries-of-web

# 4. Create a branch for your work
git checkout -b feature/your-feature-name
```

### Branch Naming Convention
```
feature/short-description        # New feature or content
fix/short-description            # Bug fix
docs/short-description           # Documentation improvement
improvement/short-description    # Enhancement to existing content
```

---

## ✨ Contribution Guidelines

### For Documentation Changes

#### Before You Start
- [ ] Read the existing documentation
- [ ] Understand the current structure
- [ ] Check for similar content
- [ ] Review CODE_STYLE.md for formatting

#### Making Changes
```markdown
# Good: Clear, concise, well-organized
# Title clearly states the topic
## Subsections for organization
- Bullet points for lists
- Code examples with language specified

# Bad: Unclear structure
Stuff about HTML
some more info
maybe a code example
```

#### Documentation Standards
- Use clear, beginner-friendly language
- Include code examples where applicable
- Add section headers for organization
- Link to related documentation
- Use consistent formatting
- Include practical exercises
- Add self-check questions

### For HTML/CSS Changes

#### Code Quality
- [ ] Follow CODE_STYLE.md guidelines
- [ ] Use semantic HTML elements
- [ ] Maintain consistent indentation
- [ ] Add meaningful comments
- [ ] Test in multiple browsers

#### Before Committing
```bash
# 1. Validate HTML
# Use online validator or HTML Tidy

# 2. Validate CSS
# Use W3C CSS Validator

# 3. Check all links work
# Test images and external links

# 4. Test accessibility
# Use WAVE or AXE tools
```

#### Commit Messages
```
# GOOD: Clear, descriptive
git commit -m "Add CSS styling guidelines to CODE_STYLE.md"
git commit -m "Fix broken link in RESOURCES.md"
git commit -m "Add example form to Activity 2"

# BAD: Vague, unclear
git commit -m "Update stuff"
git commit -m "Fixed"
git commit -m "Changes"
```

### For New Activities

#### Requirements
- [ ] Progressive difficulty level
- [ ] Clear learning objectives
- [ ] Well-commented code
- [ ] Practice exercises included
- [ ] Self-check questions
- [ ] Updated documentation
- [ ] Links to resources

#### Structure
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Activity Name</title>
</head>
<body>
    <!-- Add meaningful comments explaining the activity -->
    <!-- Each section should build on previous concepts -->
    <!-- Include at least one practice exercise element -->
</body>
</html>
```

#### Documentation Requirements
Add comprehensive documentation in ACTIVITIES.md:
- Activity title and difficulty level
- Learning objectives (3-5 items)
- Key concepts with explanations
- Code examples
- Practice exercises
- Self-check questions

---

## 🔄 Pull Request Process

### 1. Before Submitting
- [ ] Update documentation if needed
- [ ] Follow CODE_STYLE.md guidelines
- [ ] Test your changes thoroughly
- [ ] Validate HTML and CSS
- [ ] Check all links work
- [ ] Ensure accessibility standards met

### 2. Create a Pull Request
- Use a clear, descriptive title
- Include a detailed description of changes
- Reference related issues if applicable
- Include before/after examples if relevant

### PR Title Examples
```
✨ Add new CSS positioning examples to Activity 3
📝 Improve HTML best practices documentation
🐛 Fix broken image link in Activity 1
♿ Improve accessibility of Activity 4 form
```

### PR Description Template
```markdown
## Description
Brief explanation of what this PR does.

## Type of Change
- [ ] New activity
- [ ] Documentation improvement
- [ ] Bug fix
- [ ] Enhancement

## Changes Made
- Specific change 1
- Specific change 2
- Specific change 3

## Testing Done
- Tested in Chrome
- Tested in Firefox
- Validated HTML
- Checked accessibility

## Related Issues
Fixes #123
Related to #456

## Additional Notes
Any additional context or considerations.
```

### 3. Review Process
- Repository maintainers will review your PR
- Feedback will be provided within 5-7 days
- Make requested changes in new commits
- Request re-review once changes are complete
- PR will be merged once approved

### 4. After Merge
- Your contribution will be acknowledged
- Changes will appear in the next update
- Thank you for your contribution! 🎉

---

## 📐 Maintaining Consistency

### Repository Structure
```
Preliminaries-of-web/
├── README.md                          # Main overview
├── ACTIVITIES.md                      # All activity documentation
├── LEARNING_PATH.md                   # Learning progression guide
├── CODE_STYLE.md                      # Coding standards
├── CONTRIBUTING.md                    # This file
├── RESOURCES.md                       # Learning resources
├── HTML_Activity_0X_215565L.html      # Activity files
└── images/                            # Image assets
```

### File Naming Conventions
- Activities: `HTML_Activity_0X_215565L.html` (where X is the number)
- Images: Descriptive lowercase with hyphens (e.g., `hotel-bedroom.jpg`)
- Documentation: Uppercase with underscores (e.g., `CODE_STYLE.md`)

### Update Checklist
When adding new content, update:
- [ ] README.md (if adding new activity)
- [ ] ACTIVITIES.md (detailed documentation)
- [ ] LEARNING_PATH.md (progression guide)
- [ ] Any other relevant files

---

## ✅ Quality Checklist

### HTML Quality
- [ ] Valid HTML5 structure
- [ ] Proper semantic elements
- [ ] All images have alt text
- [ ] All links are descriptive
- [ ] Proper indentation (4 spaces)
- [ ] Meaningful comments
- [ ] No inline styles
- [ ] Accessible to screen readers

### CSS Quality
- [ ] Valid CSS syntax
- [ ] Consistent color format
- [ ] Proper selector naming
- [ ] Organized properties
- [ ] No unnecessary specificity
- [ ] Cross-browser compatible
- [ ] Performance optimized

### Documentation Quality
- [ ] Clear, beginner-friendly language
- [ ] Includes code examples
- [ ] Well-organized sections
- [ ] Links to related docs
- [ ] Consistent formatting
- [ ] Practical exercises included
- [ ] No typos or grammatical errors

### Accessibility
- [ ] WCAG 2.1 Level AA compliant
- [ ] Keyboard navigable
- [ ] Proper color contrast
- [ ] Alt text for images
- [ ] Semantic HTML structure
- [ ] Form labels associated
- [ ] Focus indicators visible

---

## 🚨 Common Issues and Solutions

### Issue: HTML doesn't validate
**Solution**: Use W3C Validator to identify errors
- Check for unclosed tags
- Verify proper nesting
- Confirm valid attribute values

### Issue: CSS not applying
**Solution**: Check CSS specificity and order
- Verify selectors are correct
- Check browser DevTools for conflicts
- Ensure CSS is before closing `</style>` tag

### Issue: Images not loading
**Solution**: Verify image paths and formats
- Check file exists in correct location
- Verify file path is correct
- Ensure supported image format
- Check file permissions

### Issue: Accessibility fails
**Solution**: Use WAVE or AXE browser extensions
- Add alt text to images
- Use semantic HTML
- Ensure sufficient color contrast
- Associate labels with inputs

---

## 📞 Getting Help

### Questions About Contributing?
1. Check this document first
2. Review similar existing contributions
3. Check GitHub issues for similar questions
4. Open a new issue with your question

### Questions About Content?
1. Read the relevant documentation
2. Check RESOURCES.md for learning materials
3. Comment on a relevant issue
4. Create a new issue for discussion

### Need Clarification?
- Open an issue with questions
- Include specific details
- Reference relevant files/sections
- Be respectful and patient

---

## 🎓 Learning Resources for Contributors

### HTML Best Practices
- MDN Web Docs: https://developer.mozilla.org/en-US/docs/Web/HTML
- W3C HTML Standard: https://html.spec.whatwg.org/
- Web Standards: https://www.w3.org/

### CSS Best Practices
- MDN CSS Guide: https://developer.mozilla.org/en-US/docs/Web/CSS
- W3C CSS Specifications: https://www.w3.org/Style/CSS/

### Accessibility
- WCAG Guidelines: https://www.w3.org/WAI/WCAG21/quickref/
- WebAIM: https://webaim.org/
- ARIA Authoring Practices: https://www.w3.org/WAI/ARIA/apg/

### Git and GitHub
- GitHub Guides: https://guides.github.com/
- Git Documentation: https://git-scm.com/doc
- GitHub Flow: https://guides.github.com/introduction/flow/

---

## 🏆 Recognition

### Contribution Recognition
- All significant contributions will be acknowledged
- Contributors may be listed in README.md
- Major contributions may be featured in release notes
- Thank you for making this project better!

### Levels of Contribution
- **Typo fixes**: Quick and appreciated
- **Documentation improvements**: Valuable for learners
- **New activities**: Significant expansion of content
- **Tool development**: Automation and testing improvements
- **Community support**: Helping others learn and contribute

---

## 📜 Code of Conduct

### Be Respectful
- Treat all contributors with respect
- Appreciate diverse perspectives
- Welcome new contributors

### Be Collaborative
- Provide constructive feedback
- Help others improve their contributions
- Share knowledge and expertise

### Be Professional
- Use clear, professional language
- Stay focused on technical issues
- Avoid personal attacks or comments

### Zero Tolerance
- No harassment or discrimination
- No spam or self-promotion
- No malicious code or content

---

## 📝 License

By contributing to this repository, you agree that your contributions are licensed under the same terms as the project.

---

## 🙏 Thank You

We appreciate your interest in making Preliminaries of Web better! Whether you're:
- Fixing typos
- Improving documentation
- Adding new content
- Reporting issues
- Sharing ideas

...your contribution helps make web development education more accessible to everyone. Thank you! 🎉

---

**Last Updated**: 2026-05-22

**Questions?** Open an issue on GitHub or contact the maintainers.
