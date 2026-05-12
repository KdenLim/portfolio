# Kayden Lim - Portfolio Project Manifest

Welcome to the codebase for Kayden Lim's personal portfolio! This document serves as a guide for AI coding assistants to quickly understand the project's architecture, tech stack, and design guidelines.

## 📌 Project Overview
- **Purpose**: A personal portfolio website for Kayden Lim, showcasing his experience and projects as a Data Engineer.
- **Role Persona**: Data Engineer (focus on ETL, pipelines, Snowflake, AWS, Terraform, Data Architecture).

## 🛠️ Tech Stack & Architecture
This project is intentionally built to be lightweight, blazing fast, and dependency-free.
- **Core**: Vanilla HTML5, CSS3, and JavaScript.
- **Frameworks/Build Tools**: **NONE**. Do not introduce npm, Node.js, React, Webpack, Tailwind, or any build steps.
- **Libraries**: No external JS libraries (e.g., jQuery is intentionally removed). Native Browser APIs (like Intersection Observer) are preferred.
- **Deployment**: Deployed as a static site to Cloudflare Pages.

## 🎨 Design System & CSS
The site uses a custom dark/earth-toned theme powered by CSS Variables in `styles.css`.

**Color Palette**:
- Base Background: `#A47251` (Medium Brown)
- Alt Background: `#8e6245` (Darker Brown)
- Primary Text: `#DCF0C3` (Light Green/Cream)
- Secondary Text: `#F0D8A1` (Light Tan)
- Accent Color: `#DD9E59` (Vibrant Orange)

**Guidelines**:
- Use `styles.css` for all styling.
- Maintain the use of CSS variables (`:root`) for color management.
- Typography: Uses 'Inter' for body text and 'Fira Code'/'Roboto Mono' for code/technical accents.

## 📝 Coding Guidelines
1. **Semantic HTML**: Always use proper HTML5 semantic tags (`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`, `<article>`).
2. **SEO Focus**: Ensure all images have `alt` tags. Do not use `<meta http-equiv="refresh">` redirects. Maintain high-quality Open Graph and standard meta tags in `index.html`.
3. **Accessibility**: Maintain high contrast ratios (which the current palette is designed for) and use ARIA labels where appropriate.
4. **Witty Tone**: Kayden appreciates a slightly witty, self-aware, and human tone in his copywriting (e.g., joking about getting wrecked in Brazilian jiu-jitsu or overanalyzing his Spotify listening habits). Maintain this tone when suggesting copy.

## 📁 File Structure
- `index.html`: The single-page application entry point containing all content.
- `styles.css`: All styling and design tokens.
- `main.js`: Logic for intersection observers (scroll animations) and interactive elements.
- `images/`: Directory containing all local image assets.
- `agents.md`: This file.
