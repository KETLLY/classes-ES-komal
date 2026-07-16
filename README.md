# Komal's Spanish Learning App 🇨🇴

Interactive web app to track Komal's Spanish learning journey from A2 to B1, focused on life in Bogotá, travel, culture, and work as an IT Developer.

## 🚀 How to publish this on GitHub Pages

1. Rename `komal-spanish-app.html` to `index.html`.
2. Upload it to the root of this repository (drag & drop via the GitHub web UI works fine).
3. Go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`.
5. Select branch `main` and folder `/ (root)`, then click **Save**.
6. Wait 1-2 minutes. Your site will be live at:
   `https://<your-username>.github.io/<repo-name>/`

## 🔄 How to update the content later

- Open `index.html` directly in this repo (use the pencil/edit icon on GitHub).
- The curriculum data lives inside the `<script>` tag, in the `weeks` array — each entry is `[weekNumber, theme, [classes]]`.
- To change which class is "next", update the `currentClass` variable near the top of the script.
- Commit your changes — GitHub Pages redeploys automatically within a minute or two.

## ⚠️ Known limitations

- Progress checkmarks are saved in the browser's `localStorage`, so they do **not** sync between devices (e.g., Komal's laptop vs. phone).
- This is a static site — there is no backend or database. All curriculum content is edited directly in the HTML/JS.
- For real cross-device sync of progress, a backend (Firebase, Google Sheets API, etc.) would need to be added separately.

## 📚 Structure

- **Home** — progress overview, next class highlight, student bio, scope note on realistic B1 timeline.
- **Needs** — Komal's stated goals, focus skills, languages, self-assessed level, class frequency.
- **Curriculum** — 12 weeks × 2 classes = 24 classes, each with a specific learning outcome and language content (grammar, vocabulary, functional phrases).
- **Lesson Format** — the standard 50-minute lesson structure used in every class.