# JAIN Online Landing Page

**JAIN Online Programs** — A responsive marketing landing page designed to showcase the university's online MBA / MCA / M.Com offerings, faculty, rankings, alumni stories, and lead-capture form.

![Status](https://img.shields.io/badge/status-active-success)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?logo=tailwindcss&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/license-Proprietary-blue)

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Requirements](#requirements)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Deployment](#deployment)
- [Browser Support](#browser-support)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

This repository hosts the static marketing landing page for **JAIN Online Programs** — the online learning vertical of JAIN (Deemed-to-be University). The page drives admissions enquiries for online MBA, MCA, and M.Com programs by walking visitors through the full marketing funnel: brand promise, programs, academic approach, accreditation, faculty, employer outcomes, alumni stories, and a lead-capture form.

Built as a single, dependency-light HTML file for fast page loads and effortless deployment to any static host.

## Features

- **Single-page funnel** — hero, programs, academic approach, rankings, micro-credentials, faculty, employers, testimonials, alumni, FAQ, and an "Apply Now" form
- **Fully responsive** — mobile-first layout that scales cleanly to tablet and desktop breakpoints
- **Scroll-reveal animations** — content fades in as the viewport reaches each section
- **Interactive carousels** — faculty and testimonial sliders with snap scrolling
- **Lead-capture form** — "Apply Now" CTA with client-side validation
- **Brand-aligned theming** — custom Tailwind palette (`primary`, `secondary`, `tertiary`) and Poppins / Inter typography
- **Zero build step** — open the HTML file and it just works

## Tech Stack

| Layer        | Technology                                                   |
| ------------ | ------------------------------------------------------------ |
| Markup       | HTML5 (semantic)                                             |
| Styling      | [Tailwind CSS](https://tailwindcss.com) (CDN) + inline CSS   |
| Scripting    | Vanilla JavaScript (ES6)                                     |
| Typography   | Google Fonts — **Inter** (body) & **Poppins** (headings)     |
| Dev Tooling  | [`http-server`](https://www.npmjs.com/package/http-server)   |

No frameworks, no bundlers, no package manager required.

## Requirements

- A modern browser — Chrome, Firefox, Safari, or Edge (latest two versions)
- An active internet connection (Tailwind CSS, Google Fonts, and external assets load from CDNs)
- **Node.js 14+** *(only required if using `http-server` for local development)*

## Project Structure

```
agent-jo-langing-page/
├── index.html              # Complete landing page — markup, styles, and scripts
├── README.md
└── assets/                 # Section-scoped image assets
    ├── about/
    ├── alumni/
    ├── brand/
    ├── employers/
    ├── faculty/
    ├── hero/               # hero-banner.png, logo.svg
    ├── impactful-minds/
    ├── linkedin/
    ├── micro-credentials/
    ├── programs/           # mba.png, mca.png, mcom.png
    ├── recognitions/
    └── testimonials/
```

**Page sections** (top to bottom): Hero → Programs → Academic Approach → Rankings → Micro-Credentials → Faculty → Employers → Testimonials → Alumni → Apply Now → FAQ.

## Getting Started

### 1. Clone the repository

```bash
git clone <repository-url>
cd agent-jo-langing-page
```

### 2. Run the development server

The page is fully static and served with [`http-server`](https://www.npmjs.com/package/http-server).

**Install globally (recommended)**

```bash
npm install -g http-server
```

**Start the server from the project root**

```bash
http-server -p 8000 -o
```

Then open [http://localhost:8000](http://localhost:8000). The `-o` flag opens the browser automatically.

**Run without installing**

```bash
npx http-server -p 8000 -o
```

### Useful flags

| Flag      | Purpose                                                  |
| --------- | -------------------------------------------------------- |
| `-p 8000` | Set the port (default: `8080`)                           |
| `-o`      | Open the default browser after starting                  |
| `-c-1`    | Disable caching — recommended during active development  |
| `-g`      | Enable gzip compression                                  |

Recommended command for active development:

```bash
http-server -p 8000 -o -c-1
```

## License

Proprietary — © JAIN Online. All rights reserved.
