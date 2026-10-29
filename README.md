# DeutschPath Academy Version 8 — 52-week framework

## Changes
- Repairs Week 1 navigation and adds previous/next week controls for all 52 weeks.
- Seven top-level navigation categories only; study timer is a utility at top right, not a category.
- 52-week curriculum directory with 364 daily 240-minute study plans (CSV + JSON).
- Weeks 1–3 retain the previously authored interactive lessons.
- Weeks 4–52 provide functioning guided study templates, vocabulary, speech playback, vocabulary comprehension quizzes, writing, and local progress. These are **not** 343 fully authored four-hour lessons. Expert-authored explanations, authentic audio, and skills assessments remain future work.
- Timer starts, pauses, survives reload, and can log a completed session into the existing study tracker. Elapsed wall time is not proof of focused learning.
- Existing Week 1–3 local storage keys retained. Back up before deployment.

## Deploy to GitHub Pages
Upload **all five files** from this ZIP to the root of your existing GitHub Pages repository (replace existing index.html and manifest.webmanifest): index.html, manifest.webmanifest, README.md, curriculum_52_weeks.csv, curriculum_52_weeks.json. GitHub Pages source: main branch, /(root). Refresh after deploy.

## Important limitations
- Browser text-to-speech depends on installed German voices.
- No automatic cross-device sync; progress is stored locally.
- Writing and speaking are self-reviewed, not machine graded.
- Week 4–52 guided lesson templates are a working curriculum scaffold, not certified A1–B2 course content.
- Completion does not imply CEFR proficiency.
- 4 hours per day of focused study may require additional breaks and a sustainable sleep schedule.
