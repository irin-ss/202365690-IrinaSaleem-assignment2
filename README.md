# Irina Saleem — Personal Portfolio

A personal portfolio website built with HTML, CSS, and JavaScript for SWE363,
featuring an About/Hero section, technical projects, a design gallery, skills,
and a contact form.

**Assignment 1** built the static site. **Assignment 2** (this version) adds
interactivity: project search and filters, a validated contact form, a
personalised greeting, and scroll animations.

## Live Demo
[Visit this site](https://irin-ss.github.io/202365690-IrinaSaleem-assignment2/)
to view the live demo of the portfolio.


## Folder Structure

```
202365690-IrinaSaleem-assignment2/
├── README.md
├── index.html
├── css/
│   └── styles.css
├── js/
│   └── script.js
├── img/
│   ├── Logo.png
│   ├── project1.png
│   ├── project2.png
│   ├── PowerPlay.png
│   ├── MeetnGreet.png
│   └── GamingCertificate.png
├── docs/
│   ├── ai-usage-report.md
│   └── technical-documentation.md
└── .gitignore
```

## Features

### From Assignment 1

- **About** — a short introduction and a portrait image
- **Technical Projects** — two engineering projects (MIPS processor design,
  FPGA-based VPN accelerator) with tags and links (report and source links are
  still placeholders)
- **Designs** — a hover-to-reveal gallery of posters and graphics I've designed
- **Skills** — languages, tools, and what I'm currently learning
- **Dark/light theme toggle** — remembers the visitor's choice using
  `localStorage`, and falls back to the visitor's OS-level preference on
  first visit
- **Time-of-day greeting** — the hero greeting changes between morning,
  afternoon and evening

### New in Assignment 2

| Requirement | What I added |
| --- | --- |
| **Dynamic content** | **Live project search** and **tag filter chips** (e.g. Verilog, FPGA). Chips are generated automatically from each project card's tags, and a counter shows "Showing X of Y projects" |
| **Data handling** | **Contact form validation** (name, email format, message length) with a confirmation message on success, plus `localStorage` for the theme and for the visitor's details |
| **Personalised greeting** | After a successful form submission, the visitor's name is saved in their browser, so the greeting becomes e.g. "Good evening, Irina". Name and email also pre-fill the form next time. A **"Not you? Forget my details"** button clears them |
| **Animation and transitions** | Fade-in on scroll for cards and the form, hover transitions on buttons, chips and cards, and animated error and success messages. Animations are turned off for visitors who prefer reduced motion |
| **Error handling and user feedback** | Inline error messages that say what is wrong and how to fix it, focus moves to the first invalid field, a "No projects found" empty state with a **Clear search** button, and a status message after sending |


**Note:** the contact form has no backend yet (`action="#"`). A valid
submission shows a confirmation and saves the visitor's details locally, but the
message is not actually sent.

## Setup Instructions - Run Locally

No build tools or installs are required — this is a static site.

1. **Clone the repository**
```bash
git clone https://github.com/irin-ss/202365690-IrinaSaleem-assignment2.git
cd 202365690-IrinaSaleem-assignment2
```
2. **Open it in a browser**
    - Double-click `index.html`, or
    - Open the folder in VS Code and use the "Live Server" extension, or
    - Serve it locally:
```bash
python3 -m http.server 8000
```

then visit
```
http://localhost:8000
```

### Trying the new features

1. **Search and filter:** type "FPGA" in the project search, or click a tag chip. Search for nonsense to see the empty state.
2. **Form validation:** press *Send Message* with empty fields, then with an invalid email, then with valid details.
3. **Personalised greeting:** after a valid submission, the greeting gains your first name. Refresh the page and it stays. Click *Not you?* to clear it.
4. **Theme:** toggle dark mode, refresh, and the choice is kept.

## Documentation

- [`docs/ai-usage-report.md`](docs/ai-usage-report.md) — tools used, what was changed, and what I learned
- [`docs/technical-documentation.md`](docs/technical-documentation.md) — how each JavaScript function works, data flow, and CSS notes

## AI Use (Summary)

In Assignment 1, AI assistance was used for scaffolding sections, debugging
CSS/HTML class mismatches, and reviewing spacing and layout issues.

In Assignment 2, AI (Claude) was used to help generate outlines and explain the project
search and filter, the form validation, the scroll animations and the saved-name
greeting. I reviewed, tested and edited the output, and kept my Assignment 1
code intact. Full details — tools used, what was changed, and what I learned —
are in [`docs/ai-usage-report.md`](docs/ai-usage-report.md).

## Browser Support

Tested in the latest versions of Chrome and Edge, and checked at desktop,
tablet, and mobile widths using browser DevTools.

## Author

- **Name:** Irina Saleem
- **Student ID:** s202365690
- **Course:** SWE363
