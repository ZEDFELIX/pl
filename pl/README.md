# Share Your Secret — Anonymous Stories

A lightweight anonymous story-sharing web app. Users post short stories that are stored in the browser's `localStorage` (per-device), with the ability to delete their own stories.

## Files

- `index.html` — Single page: submit form + story feed
- `styles.css` — Styling
- `script.js` — Store, render, and delete stories using `localStorage`

## How to open

Double-click `index.html` in a browser, or serve the folder locally:

```console
python -m http.server 8000
```

Then visit http://localhost:8000.

## Notes

- Stories are stored client-side only (`localStorage`); clearing browser data removes all stories. A backend/database is required for cross-device persistence.
- Each visitor gets an auto-generated anonymous `userId` used only to allow deleting their own posts.