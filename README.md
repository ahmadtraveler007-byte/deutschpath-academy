# DeutschPath Academy — Version 2.0

Static website for GitHub Pages and Hostinger. No build step required.

## Install / update GitHub Pages
1. Extract the ZIP. Upload `index.html` and `manifest.webmanifest` to the **root** of your existing `deutschpath-academy` GitHub repository, replacing the old `index.html`.
2. Keep Settings > Pages > Deploy from a branch > main > /(root).
3. Wait for the deployment and refresh your published URL with Ctrl+F5.

## Features
- Dedicated interactive Day 1: German alphabet, special letters, pronunciation rules, German-English-Urdu explanations, browser TTS, optional speech recognition (transcription only), eight-question graded quiz, saved writing assignment, and completion criteria.
- Existing Days 2–6 now open on separate pages, but retain starter-level content.
- Existing dashboard, A0 checkpoint, flashcards, roadmap, backup import/export.
- Existing localStorage progress retained using `deutschpath-progress-v1`.

## Limitations
- Local browser storage only; no cloud synchronization.
- Browser-generated audio depends on installed German voices; no pronunciation scoring.
- Writing is saved, not auto-graded.
- 52-week curriculum is a roadmap, not completed course content.
- Completion requires best quiz >=6/8 and writing >=30 characters; does not prove CEFR proficiency.
