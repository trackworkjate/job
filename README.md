# OISHI & FOA Project Timeline Dashboard

Dynamic weekly Gantt dashboard for the **New POS Software OISHI & FOA** project.

The dashboard reads the current date from the browser, calculates overall project progress, highlights the current process, and displays the full project plan in a weekly Gantt-style chart.

## Features

- Overall project completion hero section
- Current process status based on the selected date
- KPI snapshot:
  - Days passed
  - Days remaining
  - Current task progress
  - Track status
  - Upcoming milestones
- Weekly Gantt chart with 4 weeks per month
- Today marker on the chart
- Blinking current task label
- Task type legend
- Export to PDF in landscape layout

## Files

- `index.html` - Main dashboard file
- `messageImage_1779342406359.jpg` - Original timeline reference image

## How To Use

Open `index.html` in a browser.

To test a different project date, change the date picker in the top-right corner. The dashboard will update automatically.

## Export To PDF

Click **Export PDF** in the top-right corner.

Recommended print settings:

- Layout: Landscape
- Paper size: A3
- Background graphics: Enabled
- Scale: Fit to page, or 70-90% if needed

## GitHub Pages Deployment

1. Create a new GitHub repository.
2. Upload `index.html`, `README.md`, and the reference image if you want to keep it.
3. Go to **Settings > Pages**.
4. Under **Build and deployment**, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
5. Save.

After GitHub finishes deployment, the dashboard will be available at:

```text
https://<your-github-username>.github.io/<repository-name>/
```

## Local Git Setup

If this folder is not yet a git repository:

```bash
git init
git add index.html README.md messageImage_1779342406359.jpg
git commit -m "Add OISHI FOA project timeline dashboard"
git branch -M main
git remote add origin https://github.com/<your-github-username>/<repository-name>.git
git push -u origin main
```

## Updating The Dashboard

Edit `index.html`, then commit and push:

```bash
git add index.html README.md
git commit -m "Update project timeline dashboard"
git push
```

GitHub Pages will update automatically after the push.
