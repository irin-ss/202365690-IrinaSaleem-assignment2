
# Irina Saleem — Personal Portfolio

A personal portfolio website built with HTML, CSS, and JavaScript for SWE363,
featuring an About/Hero section, technical projects, a design gallery, skills,
and a contact form.

## Live Demo
[Visit this site](https://irin-ss.github.io/202365690-IrinaSaleem-assignment1/)
to view live demo of the portfolio.

## Folder Structure

```
irina-saleem-portfolio/
├── index.html
├── css/
│ └── styles.css
├── js/
│ └── script.js
├── img/
│ ├── Logo.png
│ ├── project1.png
│ ├── project2.png
│ ├── PowerPlay.png
│ ├── MeetnGreet.png
│ └── GamingCertificate.png
└── docs/
└── ai-usage-report.md

```

## Features

- **About** — a short introduction and a portrait image
- **Technical Projects** — two engineering projects (MIPS processor design,
  FPGA-based VPN accelerator) with tags and links (currently empty links)
- **Designs** — a hover-to-reveal gallery of posters and graphics I've designed
- **Skills** — languages, tools, and what I'm currently learning
- **Contact** — a form with name, email, message, and a query-type dropdown (does not work yet)
- **Dark/light theme toggle** — remembers the visitor's choice using
  `localStorage`, and falls back to the visitor's OS-level preference on
  first visit

## Setup Instructions - Run Locally

No build tools or installs are required — this is a static site.

1. **Clone the repository**
```bash
    https://github.com/irin-ss/202365690-IrinaSaleem-assignment1.git
```
2. **Open it in a browser**
    - Double-click `index.html`, or
    - Open the folder in VS Code and use the "Live Server" extension, or
    - Serve it locally:
```bash
     python3 -m http.server 8000
```

then visit 
```bash
 http://localhost:8000.
```

## AI Use (Summary)

AI assistance was used for scaffolding sections, debugging CSS/HTML class
mismatches, and reviewing spacing and layout issues. Full details — tools
used, what was changed, and what I learned — are in
[`docs/ai-usage-report.md`](docs/ai-usage-report.md).

## Browser Support

Tested in the latest versions of Chrome and Edge, and checked at desktop,
tablet, and mobile widths using browser DevTools.

## Author

- **Name:** Irina Saleem
- **Student ID:** s202365690
- **Course:** SWE363