# DeutschPath Academy V9.0 — Modular rebuild

## Important: what this release actually includes

This is a new, independently organized static web application, not another patch on the V8 monolithic `index.html`.

**Working application features:**
- Exactly seven top-level navigation categories.
- 52 clickable weeks; each opens seven clickable daily study pages (364 total).
- Previous/next week and previous/next day navigation, including Week 1.
- Five functional lesson tabs (Learn, Listen, Practice, Write, Results) for every day.
- Six example phrases per week (312 curated German–English–Urdu examples); text-to-speech depends on browser voices.
- Six-question vocabulary quizzes per day; score and attempts saved locally.
- Writing autosave and internal lesson-completion checkpoints.
- 52 weekly vocabulary checkpoints (12 questions, repeating six example phrases).
- Circular, manual Start/Pause/Save timer with current local date and running elapsed time.
- Daily, weekly (Monday–Sunday) and monthly reports with date picker; manual session entry, deletion, and complete V9 JSON backup/import.
- Responsive layout and no required CDN, Node, Python or third-party runtime.

**Curriculum depth limitation:**
The 52-week JSON/CSV provides a 364-day topic roadmap and four-hour activity plans. Weeks 4–52 contain *guided learning scaffolds*, not 343 complete, expert-reviewed four-hour teaching chapters. The quiz checks recognition of example translations, not grammatical mastery or CEFR proficiency. Week 1–3 are also rebuilt using this new consistent teaching structure; they do not exactly replicate the longer V3/V4 lesson text. A complete, expert-reviewed A0–B2 curriculum would require additional authored readings, exercises, audio, speaking assessment, feedback and graded mock exams.

## File structure

- `index.html`: accessible HTML shell.
- `assets/css/styles.css`: responsive design.
- `assets/js/app.js`: router, UI, timer, reports, quiz logic and storage.
- `assets/js/data.js`: curated vocabulary phrase banks and learning schedules.
- `data/curriculum.json`: 364-day roadmap (loaded with fetch).
- `data/curriculum_364_days.csv`: spreadsheet-friendly export.
- `manifest.webmanifest`: web-app metadata.
- `README.md`: this file.

## GitHub Pages installation

1. Export your progress from the old site before upgrading; **V8 backup files are not directly compatible with the V9 importer**.
2. Download and extract this ZIP.
3. In your existing GitHub repository, upload `index.html`, `assets/`, `data/`, `manifest.webmanifest` and `README.md` at the repository root. Preserve folders and their contents. **Do not upload only `index.html`.**
4. Remove outdated website files if they conflict with this structure. Commit.
5. Settings → Pages → Deploy from branch → `main` → `/ (root)`.
6. Wait for deployment and hard-refresh (Ctrl+F5).
7. Test Lessons → Week 1 → Day 1; Next Week → Week 2; Week 52; Start/Pause/Save; My Progress calendar.

If GitHub's browser upload does not preserve the folders as intended, create folders with GitHub's file editor or use GitHub Desktop to commit the extracted directory. Ensure `assets/js/app.js` and `data/curriculum.json` resolve from the published URL.

## Hostinger installation

Upload the *contents* of this directory (including `assets` and `data`) to `public_html/deutschpath/` or your desired subdirectory, using File Manager or FTP. Visit `https://yourdomain.example/deutschpath/`. A regular static web host is sufficient. No PHP/Python server or database is needed for this version.

## Study timer & privacy

- The timer starts **only** when you click Start.
- Pause stops counting. Save records the elapsed time on the browser's current local date.
- If the tab is refreshed while running, elapsed time is recovered from the saved start timestamp. If you leave it running, elapsed time continues until you pause/save.
- Date reports are calculated from manually recorded sessions.
- All data is in `localStorage` **for that browser and exact website origin**, not on GitHub, Hostinger's server or a database. Changing domains/devices/browsers does not synchronize records.
- Use My Progress → Download complete JSON backup regularly; import on another device as needed.
- The legacy completion import is a best-effort tool and may not recognize every older release's data layout. It does not import old quiz scores or writing.

## QA status

- Node JavaScript syntax validation passed.
- Curriculum data validated: 52 weeks, 364 unique days, 240-minute daily schedules.
- Browser smoke tests using Chromium with an injected data source and mock browser storage passed for Week 1, Week 2, Week 3, Week 52, navigation, timer save, reports and exam directory.
- Live GitHub Pages / Hostinger deployments and browser audio are **not** verified by these tests.

## Future production enhancements

For true cross-device accounts and secure server-side records, a backend (e.g. Supabase or Hostinger PHP + MySQL) is required. GitHub Pages cannot execute PHP or Python server code. Any backend requires authentication, authorization and security review before use. Keep this version fully static for maximum deployment compatibility.


## Version 10.0 additions
- Seven top-level navigation categories remain unchanged.
- Every week now has a dedicated **Extra resources** button and every daily lesson has an **Extra** tab.
- Extra links include DW, Goethe-Institut, VHS-Lernportal, Easy German, official YouTube film and topic search pages. External links open on their providers; PDFs are **not redistributed**.
- Dashboard offers 4-hour (240 minute) core or 5-hour (300 minute) study target. The optional extra hour is divided into video, podcast and reading/shadowing.
- All 364 days have expanded guided assignments and an updated curriculum JSON/CSV. This is **not 364 expert-authored textbook lessons**.
- Existing Version 9 localStorage keys are preserved for progress and study sessions. New extra notes use the existing backup state.
- Do not upload only index.html. Upload assets/ and data/ preserving directory structure.
