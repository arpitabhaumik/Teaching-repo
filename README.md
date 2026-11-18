# Teaching Resources

This repository contains interactive classroom activities designed to help students practise key skills through short, browser-based games and quizzes.

## Repository structure

```text
Teaching-repo/
├── README.md
├── activities/
│   ├── index.html
│   ├── india-state-capitals/
│   │   └── index.html
│   └── tables/
│       └── index.html
└── .github/
    └── workflows/
        └── deploy-activities.yml
```

### What each part does

- **`README.md`** — explains the project and how the repository is organised.
- **`activities/index.html`** — the activities homepage. It lists the available activities and links students to each one.
- **`activities/<activity-name>/index.html`** — the files for an individual activity. Each activity has its own folder; its `index.html` is the page students open.
- **`.github/workflows/deploy-activities.yml`** — GitHub Actions workflow that publishes the contents of the `activities/` folder to GitHub Pages.

## Current activities

| Activity | What students practise | Page |
|---|---|---|
| **India State Capitals** | Identify Indian states and their capitals using a map-based activity. | [Open activity](https://arpitabhaumik.github.io/Teaching-repo/activities/india-state-capitals/) |
| **Times Tables Challenge** | Practise multiplication tables with questions, feedback, and a score summary. | [Open activity](https://arpitabhaumik.github.io/Teaching-repo/activities/tables/) |

## Adding a new activity

1. Create a folder inside `activities/` using a short, descriptive name (for example, `fractions`).
2. Add an `index.html` file inside that folder. The activity can keep its HTML, CSS, and JavaScript together in that file, or use additional files stored in the same activity folder.
3. Add a card or link for the new activity to `activities/index.html`, so students can find it from the activities homepage.
4. Include a link back to the activities homepage in the new activity, consistent with the other activity pages.
5. Commit and push the changes to the `main` branch.

## Publishing

GitHub Actions automatically deploys the `activities/` folder to GitHub Pages when files under `activities/` change on the `main` branch. The workflow can also be started manually from the **Actions** tab using **Deploy classroom activities to GitHub Pages**.

Once deployment completes, the activities homepage is available at:

**[https://arpitabhaumik.github.io/Teaching-repo/activities/](https://arpitabhaumik.github.io/Teaching-repo/activities/)**

The repository's source files remain in GitHub; GitHub Pages serves the published activity pages from the `activities/` folder.
