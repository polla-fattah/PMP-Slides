# PMP Exam Prep: Project Management Principles and Tools Slide Compilation

This is a series of lectures on project management principles, methods, and tools. This project covers essential topics for both project management professionals and those preparing for the PMP exam. Each lecture is designed to build a deep understanding of project management domains, from planning and execution to measurement and control. With the tools and strategies discussed here, you’ll be equipped to handle the complexities of real-world projects and succeed in the PMP exam.

## Lecture Overview

### Lecture Topics

1. **Introduction to Project Management**: Covers foundational project management concepts.
2. **Development and Life Cycle Performance Domains**: Different project life cycle models and when to use them.
3. **Planning and Execution**: Best practices for organizing and executing project work.
4. **Risk and Uncertainty Management**: Strategies for handling unpredictability in projects.
5. **Delivery and Quality Control**: Ensures projects deliver value through quality outputs.
6. **Stakeholder Engagement**: Techniques for managing stakeholder expectations and involvement.

Each lecture is presented in Markdown format and is compiled into slides using Marp, a Markdown Presentation Ecosystem. Below, you’ll find a guide to setting up Marp, using it to compile the lectures, and enhancing presentations with themes, styles, and images.

---

## Using Marp for Presentation Compilation

Marp enables you to write presentations in Markdown and export them to PDF or other formats. Follow these steps to install Marp and compile your lecture slides.

### Installation Guide

#### Windows Installation

1. **Install Node.js**: Marp is built on Node.js, so install it from [nodejs.org](https://nodejs.org/).
2. **Install Marp CLI**: Open Command Prompt or PowerShell, and enter:

```bash
   npm install -g @marp-team/marp-cli
```

#### Linux Installation

1. **Install Node.js**:

```bash
   sudo apt update
   sudo apt install nodejs npm
```
   
1. **Install Marp CLI**:

```bash
   npm install -g @marp-team/marp-cli
```

Verify Marp installation with:

```bash
    marp --version
```

---

## Compiling Slides with Marp

Once Marp is installed, you can compile your Markdown lecture files to PDF.

### Single File Compilation

To compile a single Markdown file (e.g., 'lecture.md') to PDF:

```bash
    marp lecture.md --pdf
```

### Batch Compilation

To compile all Markdown files in a directory:

```bash
    for file in *.md; do marp "$file" --pdf; done
```

### Specifying Output Destination

To save output in a specific directory:

```bash
    marp lecture.md -o ./output/lecture.pdf
```

For multiple files with specified output:

```bash
    for file in *.md; do marp "$file" -o "./output/${file%.md}.pdf"; done
```

---

## Enhancing Presentations with Images and Styles

### Adding Images

To include images in your slides:

```markdown
    ![Alt text](path/to/image.png)
```

- Ensure images are in compatible formats like PNG or JPEG.
- Use relative paths for local images or URLs for web-based images.

### Styling Slides

Marp allows styling through themes and inline CSS. Define themes in the front matter of your Markdown file.

```markdown
---
marp: true
theme: uncover
---
```

#### Additional Styling Options

1. **Background Color**:

```markdown
   <!-- Background color example -->
   class: lead
   background-color: #f0f0f0
```

2. **Custom CSS**:

```markdown
   <style>
   h1 { color: #4CAF50; }
   </style>
```

---

## Using Marp with VS Code

For a seamless workflow, use Marp with **Visual Studio Code (VS Code)**.

### Setup and Usage

1. **Install Marp for VS Code**:
   - Open the Extensions view ('Ctrl+Shift+X') and search for **Marp for VS Code**.
   - Click **Install**.

2. **Markdown Preview**:
   - Open your Markdown file and press 'Ctrl+K V' to see the Marp preview pane.

3. **Exporting to PDF**:
   - Use the export option in the Marp preview pane to save your slides directly to PDF.

4. **Using Themes in VS Code**:
   - Specify themes in the front matter (e.g., 'gaia', 'uncover').

---

## Best Practices for Marp and Markdown Presentations

1. **Organize Assets**: Store Markdown, images, and other assets in folders like 'slides/', 'images/' for easy access.
2. **Clear, Concise Slide Titles**: Keep slide titles short and focused for readability.
3. **Consistent Design**: Use a consistent font, color scheme, and background.
4. **Image Optimization**: Compress images for faster loading and improved export quality.
5. **Modularize Large Presentations**: Split large slideshows into multiple files for easier management.
