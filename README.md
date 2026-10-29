# DeutschPath Academy — Version 4.0

Static, no-build website for GitHub Pages and Hostinger.

## Included
- 7 dedicated Week 1 lessons with German–English–Urdu material. Days 2–7 now include extended teaching explanations, dialogues, audio practice and independent drills.
- Existing interactive practice questions and locally saved writing assignments.
- Separate randomized 18-question Week 1 assessment, with feedback **after submission**.
- Manual study-session tracker, skill totals and weekly assessment history.
- Export/import progress, compatible with prior v3 data under `deutschpath-progress-v1`.

## Known limits
- Day 1 keeps its original detailed lesson flow; the new deep-dive expansion targets Days 2–7.
- Lesson practice quizzes remain guided and show answers. They still control individual lesson completion; the independent weekly exam is an additional assessment.
- Writing checklist is self-review; writing is **not** grammar-graded. The 30-character completion rule measures length only.
- Speech uses browser text-to-speech and may lack a German voice.
- Progress is stored only in the browser; it is not synchronized across devices.
- 52-week roadmap is planned; only Week 1 is populated.
- Browser testing is required after deployment.

## Update your existing GitHub Pages site
1. Export a progress backup from Roadmap > Export.
2. Extract ZIP. Upload `index.html`, `manifest.webmanifest`, and `README.md` to the **root** of your existing `deutschpath-academy` GitHub repository, replacing prior versions.
3. Commit changes; GitHub Pages remains set to main / root.
4. Wait for deployment and refresh with Ctrl+F5.
5. Test Days 1–7, Weekly Exam, study logging and backup export.

For Hostinger, upload the same files to the chosen subdomain's document root, without overwriting WordPress.
