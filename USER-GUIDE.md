# Qorix Sprint Capacity Calculator - User Guide

> Full usage guide for the browser-based Qorix sprint capacity planner.

## 1. Introduction

The Qorix Sprint Capacity Calculator is a static browser app that helps teams plan sprint capacity, manage availability, and export a printable report.

Use it when you need to:

- Capture sprint metadata
- Add team members and allocate productivity
- Mark leave, holidays, and working days by date
- Review capacity totals and productivity
- Export a CSV backup or print a PDF-style report

## 2. Main Areas

The app has four main sections:

- **Dashboard** - summary metrics and sprint details overview
- **Configuration** - required sprint data and project metadata
- **Team Capacity** - member setup, daily planning, and capacity details
- **Export PDF** - printable report and CSV export

## 3. Configuration

Open **Configuration** and fill in the required fields:

- Program / Project Name
- Team / Module Name
- Sprint Number
- Sprint Name

Recommended values:

- Start Date
- End Date
- Working Days in Sprint
- Hours per Day

Optional values:

- Scrum Master
- Product Owner

Click **Save Configuration** after entering the values.

If required fields are missing, CSV/PDF output may not reflect a complete plan.

## 4. Team Capacity

### Add a Team Member

1. Open **Team Capacity**.
2. Click **+ Add Team Member**.
3. Enter:
   - Name
   - Role
   - Allocation %
   - Productivity Factor %
4. Click **Save**.

### Edit a Team Member

1. In the team planner, click **Edit** for the member.
2. Change name, role, allocation, or productivity factor.
3. Save the update.

### Productivity Factor

- Productivity factor is capped at 95%.
- It reduces the available capacity for that member.
- Use it when a member is not fully productive for the full sprint.

## 5. Daily Planning

The team planner is date-wise.

For each member and each sprint date, choose one of these states:

- `-` - no override
- Full Day - working day
- Half Leave - half day leave
- Leave - full-day leave
- Holiday - public holiday

The planner updates the member totals and the dashboard after each save.

## 6. Capacity Calculations

The app calculates:

- Working Days
- Holidays
- Leaves
- Available Days
- Available Hours
- Productivity Factor

The final available days for a member are reduced by the selected daily statuses and then scaled by allocation % and productivity factor.

## 7. Dashboard

The dashboard shows:

- Program / Project
- Team / Module
- Sprint Number
- Sprint Name
- Total Team Members
- Total Capacity in Days
- Total Capacity in Hours
- Avg Daily Capacity
- Productivity Factor

Use the dashboard for a quick planning check before exporting or sharing the plan.

## 8. Export and Import

### Export CSV

Use **Export CSV** to download the sprint configuration and team data as a CSV file.

### Export PDF

Use **Export PDF** to open the report page and print or save as PDF.

### Import CSV

Use **Import CSV** to load a previously exported CSV file back into the app.

## 9. Reset

The top-right **Reset** button clears saved configuration and team data.

Use it when you want to start a fresh sprint plan.

## 10. GitHub Deployment

### Recommended Setup

1. Place `index.html`, `README.md`, `QUICK-START.md`, and `USER-GUIDE.md` in the repository.
2. Commit and push the branch to GitHub.
3. Go to **Settings > Pages** in the repository.
4. Select the publishing branch and the root folder.
5. Save and wait for GitHub Pages to build the site.

### Deployment Tips

- GitHub Pages works best when `index.html` is at the repo root.
- Because this app is static, no build step is needed.
- If you keep the project in a folder name with spaces, test the final Pages URL carefully.

## 11. Troubleshooting

### Export does not download

- Check browser download permissions.
- Disable popup or download blockers.
- Try Chrome or Edge.

### Data seems lost after refresh

- The app stores data in browser `localStorage`.
- Avoid private browsing mode.
- Export CSV before clearing browser data.

### Totals look wrong

- Confirm start and end dates are valid.
- Check team member allocation and productivity factor.
- Review the date-wise planner for holidays and leave overrides.

## 12. Best Practices

- Fill required fields before planning capacity.
- Set dates before adding member availability.
- Keep allocation realistic for shared resources.
- Use Reset only when starting a new sprint.
- Export CSV after finishing a planning session.

## 13. Support

For a short setup path, open [QUICK-START.md](QUICK-START.md). For the product summary, open [README.md](README.md).
