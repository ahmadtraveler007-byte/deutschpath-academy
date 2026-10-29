# DeutschPath Academy — Starter Release

## Included
- Responsive static website (no build step)
- Six original A0 beginner lessons with German/English/Urdu examples and assignments
- 10-question graded checkpoint with saved best score
- 12 vocabulary flashcards with mastery tracking
- Browser German speech synthesis (voice quality depends on browser/installed voices)
- Progress tracking using localStorage; JSON export/import
- 52-week roadmap overview (not 52 weeks of lessons)

## Hostinger deployment
1. Create a subdomain, such as `learn.example.com`, in Hostinger and identify its document root.
2. Upload `index.html` and `manifest.webmanifest` directly into that document root using File Manager or FTP.
3. Visit the HTTPS URL and test lessons, assessment, and progress.
4. Do not overwrite an existing WordPress root. Use a separate subdomain/directory.

## GitHub Pages deployment
1. Create a GitHub repository and upload both files to its root.
2. In Settings > Pages, select Deploy from a branch, choose `main` and `/ (root)`.
3. Open the published Pages URL. No build is required.
4. For a custom domain, follow GitHub Pages DNS and HTTPS instructions.

## Limitations / next phases
- Progress is local to the browser; it does not sync between devices. Export/import backup is provided.
- No account system, cloud database, AI tutor, speech assessment, offline service worker, or admin editor.
- A1/A2/B1/B2 lesson content, full daily curriculum, and external mock exams are planned, not included.
- Browser speech synthesis is not prerecorded native-speaker audio.
- Completion tracking does not certify CEFR proficiency.
- Requires browser localStorage enabled; clearing site data removes progress unless backed up.
