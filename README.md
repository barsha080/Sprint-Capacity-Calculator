# Qorix Sprint Capacity Calculator

> A single-file, browser-based sprint capacity planner for Qorix teams.

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Browser](https://img.shields.io/badge/browser-Chrome%20%7C%20Edge%20%7C%20Firefox%20%7C%20Safari-green)
![Deployment](https://img.shields.io/badge/deployment-GitHub%20Pages-purple)

## Overview

The Qorix Sprint Capacity Calculator is a static HTML application that helps you plan sprint capacity, track team availability, and export a clean report for sharing.

It is designed to run without a backend, save data in the browser, and be deployed directly to GitHub Pages.

## What It Does

- Captures required sprint metadata: Program / Project, Team / Module, Sprint Number, Sprint Name
- Stores sprint dates, working days, hours per day, Scrum Master, and Product Owner
- Manages team members with role, allocation %, and productivity factor up to 95%
- Supports a date-wise team planner for working days, half-day leave, full-day leave, and holidays
- Calculates capacity, available days, available hours, and productivity factor
- Exports CSV for spreadsheet use
- Prints a PDF-ready report from the Export PDF page
- Imports CSV data back into the planner
- Includes a reset action to clear configuration and team data

## Files

- `index.html` - Main application
- `README.md` - Project overview and deployment instructions
- `QUICK-START.md` - Fast setup steps
- `USER-GUIDE.md` - Full usage guide

## Run Locally

1. Open `index.html` in a modern browser.
2. Enter the required sprint details in Configuration.
3. Add team members in Team Capacity.
4. Review the dashboard, export CSV, or print the PDF report.

No install step is required.

## GitHub Deployment

### Option 1: GitHub Pages from the repository root

1. Put `index.html` and the three docs at the root of the GitHub repository.
2. Commit and push to GitHub.
3. In GitHub, open **Settings > Pages**.
4. Set the source to the branch you want to publish, usually `main`.
5. Select the root folder and save.
6. Open the Pages URL after GitHub finishes publishing.

### Option 2: Deploy as a folder

If you keep the project in a folder such as `Sprint Capacity Planning`, publish that folder as the site root or copy its contents to the repository root before enabling Pages.

### GitHub Notes

- GitHub Pages works best with a root-level `index.html`.
- If you keep spaces in folder names, URLs will need encoding when accessed directly.
- Since the app is static, no build step is required.

## Browser Support

- Chrome
- Edge
- Firefox
- Safari

## Data Storage

- All saved data stays in `localStorage` in the browser.
- Use Export CSV as a backup before clearing browser data.
- Use Reset only when you want to clear the current plan.

## Support

If you need the full workflow, open [QUICK-START.md](QUICK-START.md) for the short setup path or [USER-GUIDE.md](USER-GUIDE.md) for the detailed guide.
