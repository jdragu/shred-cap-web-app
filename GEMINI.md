# Project: ShredCap Static Prototype (GEMINI.md)

This document provides an overview of the ShredCap project, reflecting its current state as a static HTML/CSS/JS prototype, and serves as instructional context for future interactions with the Gemini agent.

## Project Overview

ShredCap is a web application prototype designed to help skiers and snowboarders plan trips to Mt. Hood, Oregon. The current version is a static website demonstrating the intended user interface and aesthetic.

The project features three main pages:
*   **Home (`index.html`):** An introductory page.
*   **About (`about.html`):** Details the mission and inspiration behind ShredCap.
*   **Forecast (`forecast.html`):** Displays a simulated weather forecast table and a historical data chart for Timberline Lodge.

### Aesthetic & Vibe

The design adheres to a "Y2K Grunge" aesthetic, aiming for a "punk rock/alt rock feel" and an "early 2000s surfer vibe," blending nostalgia with a modern, tech-savvy approach. This is achieved through:
*   A dark, textured background using layered CSS `background-image` properties (user photos + grunge textures).
*   Semi-transparent dark content cards (`.content-card`) that provide a readable surface over the complex background, often with subtle rotations for a "zine" or "collage" effect.
*   Specific typography: `Permanent Marker` for display/headings and `Roboto Mono` for body/monospace text, reflecting a DIY, raw, yet digital feel.
*   A color palette primarily consisting of dark gray (`--bg-dark`), off-white (`--text-light`), and an accent teal (`--accent-teal`).

## Technologies Used

*   **Frontend:** HTML5, CSS3, JavaScript.
*   **Charting:** Chart.js (a JavaScript library for data visualization).

All CSS and JavaScript are embedded directly within the `<head>` and `<body>` tags of each respective HTML file. This project does not currently use any frontend frameworks (e.g., React, Next.js) or build tools.

## Building and Running

This is a static HTML project and requires no special build steps.

To view the website:
1.  Open `index.html` (or `about.html`, `forecast.html`) directly in any modern web browser.
2.  Ensure that all image assets (user-provided `*.JPG` files and `Grunge/*.jpeg` files) are present in their correct relative paths to the HTML files for the backgrounds to render correctly.

## Development Conventions

*   **Structure:** Each page is a standalone HTML file (`index.html`, `about.html`, `forecast.html`).
*   **Styling:**
    *   CSS is embedded within a `<style>` block in the `<head>` of each HTML file.
    *   CSS variables are used to maintain a consistent color palette and typography.
    *   The background design is central to the aesthetic, using multiple `background-image` layers, `background-blend-mode`, `filter`, and `background-attachment: fixed`.
    *   Content is placed within `.content-card` elements, which are semi-transparent dark boxes with subtle rotation and shadow effects.
*   **Scripting:** JavaScript is embedded in a `<script>` block before the closing `</body>` tag of `forecast.html` for Chart.js initialization.
*   **Assets:** Images (user-provided `*.JPG` files and `Grunge/*.jpeg` texture images) are directly referenced using relative paths.
*   **Data (Forecast Page):** The forecast table and historical chart on `forecast.html` currently use hardcoded, synthetic data. There is no API integration in this static prototype.

## Future Development (Based on original README)

While the current implementation is static, the original vision included:
*   Transitioning to a full-stack Next.js (React/Node.js) application.
*   Integrating with external weather databases (e.g., Open-Meteo API) for real-time and historical data.
*   Expanding to cover more ski resorts.

---
**Note:** This `GEMINI.md` reflects the project's state as of the last interaction and supercedes outdated information in `README.md` regarding technologies and implementation.