# DeutschPath Academy V6 — Unified Weeks 1–2
Static HTML/CSS/JavaScript website for GitHub Pages or Hostinger. No build step.

## Features
- Week 1: seven interactive lessons, 18-question Week 1 exam, study log and vocabulary.
- Week 2: seven interactive lessons (Days 8–14) with listening, practice, writing and results.
- Week 2: new independent 18-question examination.
- Unified dashboard progress: 14 published lessons.
- My Progress: Week 1 + Week 2 completion and a complete JSON backup/restore.
- Existing browser data keys retained: `deutschpath-progress-v1` and `deutschpath-week2-v1`.

## Install on GitHub Pages
1. Export a backup from the currently published site before updating.
2. Extract ZIP. Upload `index.html` and `manifest.webmanifest` to repository root, replacing the previous versions.
3. Commit changes. GitHub repository Settings > Pages > Deploy from a branch > main > /(root).
4. Wait for deployment; hard refresh (Ctrl+F5).
5. Test Week 1, Week 2, Week 2 Exam, and My Progress.

## Limitations
- Browser-local storage only; no automatic device synchronization.
- Browser text-to-speech varies by device.
- Writing is not automatically graded for German grammar.
- 52-week roadmap is a plan; 14 days are implemented.
- The Week 2 exam is an internal multiple-choice checkpoint, not a recognized CEFR assessment.
- Static syntax and archive tests do not substitute for live browser testing.

## Caution
Do not upload the ZIP itself to the repository as a website; extract and upload the files.
