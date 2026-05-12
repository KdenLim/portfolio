# Future Improvements Specification (`spec.md`)

This document outlines potential future enhancements, features, and optimizations for Kayden Lim's portfolio website. These improvements aim to showcase advanced data engineering skills, improve user experience, and increase interactivity while maintaining the lightweight ethos of the site.

## 1. Interactive Data Visualizations
**Concept:** As a Data Engineer, static images of dashboards (like Tableau) are good, but live data is better.
**Implementation:**
- Fetch data from a live backend (like the MySQL database populated by the Spotify ETL pipeline) via a simple serverless API (e.g., Cloudflare Workers).
- Use a lightweight charting library like `Chart.js` or `D3.js` to render live "Currently Listening To" or "Weekly Top Artists" charts directly in a new section.

## 2. Dynamic Content via APIs
**Concept:** Automatically keep the portfolio fresh without manual HTML edits.
**Implementation:**
- **GitHub Integration:** Use the GitHub REST API to fetch and display the 3 most recently updated repositories or showcase live commit activity.
- **Blog/Articles:** If Kayden starts writing on Medium or DEV.to, use their RSS feeds or APIs to pull the latest article titles and links into a new "Writing" section.

## 3. Serverless Contact Form
**Concept:** The current `mailto:` link is clean but can expose the email address to spam bots and adds friction for users without a default mail client.
**Implementation:**
- Build a lightweight HTML `<form>` in the footer or contact section.
- Wire the form up to a serverless form handler like Formspree or Cloudflare Pages Functions to process submissions and email them to `hello@kaydenlim.com` securely.

## 4. Theme Toggle (Light/Dark Mode)
**Concept:** Give users control over their viewing experience while showcasing basic frontend interactivity.
**Implementation:**
- Add a toggle button (e.g., a sun/moon icon) in the navigation bar.
- Write a small JavaScript function to toggle a `light-theme` class on the `<body>`.
- Update `styles.css` with a media query `(prefers-color-scheme: dark)` and override the CSS variables for the light theme to ensure accessibility and high contrast.

## 5. Privacy-Focused Analytics
**Concept:** Track portfolio engagement (which projects are clicked most, where traffic comes from) without using bloated, privacy-invasive trackers like Google Analytics.
**Implementation:**
- Integrate a lightweight, cookie-less analytics script (e.g., Plausible Analytics or Cloudflare Web Analytics).
- Use the data to iteratively improve the layout and content of the portfolio over time.

## 6. Resume PDF Viewer
**Concept:** Instead of forcing a direct download of the resume, allow users to view it directly in the browser.
**Implementation:**
- Create a dedicated `/resume.html` page.
- Embed the PDF using a simple `<embed>` or `<iframe>` tag, or render it using `pdf.js` for a more custom, branded experience.
