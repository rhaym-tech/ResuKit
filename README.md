# ResuKit

A lightweight, modular LaTeX resume template framework designed for clean, professional resumes with ATS (Applicant Tracking System) compatibility following Harvard's Bullet Point resume style.

## Features

- **Customizable Styling** – Centralized configuration for fonts, colors, spacing, and layout
- **Modular Content** – Separate files for sections (header, education, experience, projects, skills)
- **ATS-Friendly** – PDF optimizations to ensure compatibility with applicant tracking systems
- **Professional Design** – Clean typography using Charter font with proper spacing and formatting
- **Easy to Maintain** – Separation of concerns makes updates and modifications straightforward

## Quick Start

### Prerequisites
- LaTeX distribution (TeX Live, MikTeX, or MacTeX)
- A LaTeX editor (Overleaf, VS Code with LaTeX Workshop, or command line)

### Basic Usage

1. **Prepare your resume folder** by creating an empty folder as a workspace. The workspace folder must contain the ResuKit folder.

2. **Create your resume** by creating a new main .tex file to import the framework and start working, or simply use the example template attached (main file is example.tex and details are in the /content folder)

You can either to separate content in different files or use only one file.

## Project Structure

```
.
├── ResuKit/
│   ├── config/
│   │   ├── page.tex           # Page geometry and margins
│   │   ├── headings.tex       # Section heading styles
│   │   ├── lists.tex          # List formatting
│   │   ├── components.tex     # Reusable commands and environments
│   │   └── pdf.tex            # PDF optimization settings
│   └── resume.sty             # Main style package
│
├── content/
│   ├── header.tex             # CV header (name, contact)
│   ├── education.tex          # Education entries
│   ├── experience.tex         # Work experience entries
│   ├── projects.tex           # Project showcase
│   └── skills.tex             # Skills section
└── example.tex                # Example resume template (main file)
```

## Customization

### Styling Changes
Modify the configuration files in `ResuKit/config/` to adjust:
- Page margins and layout
- Section heading styles and colors
- List item formatting
- PDF metadata and settings

### Adding Sections
Add new `\input{content/your_section}` to your resume file and create the corresponding file in the `content/` directory. Or straight in your main file.

### Reusable Commands
Check `ResuKit/config/components.tex` for available commands and environments to structure your resume content.

## Building

**Command line:**
```bash
pdflatex example.tex
```

**Overleaf:**
Upload the entire folder or sync your GitHub repository directly.

**VS Code with LaTeX Workshop:**
Open `example.tex` and use the LaTeX Workshop extension to build and preview.

## Tips for ATS Compatibility
Check full article in [Harvard College Guide to Creating a Strong Resume](https://careerservices.fas.harvard.edu/resources/create-a-strong-resume/#tips).

## Contributing
Contributions are welcome! Feel free to submit improvements or bug fixes.
