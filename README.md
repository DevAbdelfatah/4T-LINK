# 4T-LINK — URL Risk Analyzer

<p align="center">
  <strong>Analyze suspicious URLs. Understand potential risks. Browse smarter.</strong>
</p>

<p align="center">
  A lightweight, responsive URL analysis tool built with HTML5, Tailwind CSS, and vanilla JavaScript.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/No_Backend-Available-70f0c0?style=for-the-badge" alt="No backend required" />
</p>

---

## Overview

**4T-LINK** is a front-end URL risk analyzer designed to identify suspicious URL patterns and help users understand potential phishing indicators before visiting a website.

The application runs its analysis locally in the browser without requiring a backend server, database, or API key.

> **Security notice:** 4T-LINK currently performs heuristic URL analysis only. It does not query threat-intelligence databases and cannot confirm whether a URL is safe or malicious.

## Features

- **URL Validation** — Validates URL structure and supported protocols.
- **Phishing Indicators** — Detects selected suspicious keywords and URL patterns.
- **Hostname Analysis** — Identifies IP-based URLs, internationalized domain indicators, and unusually structured hostnames.
- **HTTPS Awareness** — Flags HTTP URLs that do not use HTTPS.
- **Suspicious Pattern Detection** — Checks selected URL characteristics that may warrant further investigation.
- **Risk Scoring** — Calculates a heuristic indicator based on predefined rules.
- **Detailed Reports** — Displays detected indicators and their explanations.
- **Copyable Results** — Copies the analysis report to the clipboard.
- **Responsive Interface** — Supports desktop, tablet, and mobile screens.
- **Arabic RTL Interface** — Includes the Cairo font and right-to-left layout.
- **Privacy-Oriented Design** — Does not intentionally send submitted URLs to a scanning server.

## Technology Stack

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Custom styling and animations |
| Tailwind CSS | Responsive utility-based styling |
| Vanilla JavaScript | URL parsing, analysis, and report generation |
| Lucide | SVG interface icons |
| Google Fonts — Cairo | Arabic typography |

## Getting Started

### Prerequisites

- A modern web browser.
- An internet connection to load the external font, Tailwind CSS CDN, and Lucide icons.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR-USERNAME/4T-LINK.git
   ```

2. Open the project folder:

   ```bash
   cd 4T-LINK
   ```

3. Open `index.html` in your browser.

No package installation, backend server, or API key is required for the current version.

Replace `YOUR-USERNAME` with your actual GitHub username.

## How It Works

1. The user enters an HTTP or HTTPS URL.
2. JavaScript validates and parses the URL without navigating to it.
3. Local heuristic rules inspect selected URL characteristics.
4. The application calculates a risk indicator based on the detected patterns.
5. The interface displays the findings and generates a copyable report.

## Project Structure

```text
4T-LINK/
├── index.html
└── README.md
```

The current implementation keeps the HTML, CSS, and JavaScript in a single file for simple setup and deployment.

## Security Limitations

4T-LINK is an educational front-end analysis project, not a complete malware detection system.

- It does not query VirusTotal, Google Safe Browsing, or other threat-intelligence services.
- It does not inspect website content, downloaded files, redirects, or server responses.
- Its risk score is a heuristic indicator, not a probability of malicious activity.
- A low score does not establish that a URL is safe.
- False positives and false negatives are possible.
- External CDN resources are loaded when the application has internet access.

**Never rely on heuristic analysis alone when handling suspicious links.**

## Roadmap

- [ ] Integrate a threat-intelligence API through a secure backend.
- [ ] Add reputation checks from multiple security providers.
- [ ] Improve internationalized domain and homograph detection.
- [ ] Add automated tests for URL parsing and risk rules.
- [ ] Improve accessibility and offline asset handling.
- [ ] Add optional scan history with privacy controls.

Roadmap items are planned improvements and are not available in the current implementation unless explicitly marked as completed.

## Author

**Abdelfatah Abdelhamid (DEBO)**

Programming & Development

## Acknowledgements

- [Tailwind CSS](https://tailwindcss.com/)
- [Lucide Icons](https://lucide.dev/)
- [Google Fonts — Cairo](https://fonts.google.com/specimen/Cairo)

---

*Built as a front-end cybersecurity learning and portfolio project.*

