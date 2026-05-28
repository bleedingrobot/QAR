# NZC + QAR Generator

A single-file web app for New Zealand teachers to upload a reading PDF/image and generate:

- New Zealand Curriculum (NZC) alignment links
- QAR (Question-Answer Relationship) questions

Built for free hosting on GitHub Pages.

## Features

- Single-file architecture (`index.html`)
- Tailwind CSS via CDN
- Vanilla JavaScript only
- Drag-and-drop upload for `.pdf`, `.png`, `.jpg`, `.jpeg`
- Gemini API key input saved in browser `localStorage`
- In-browser Base64 conversion (no backend)
- Multimodal request to `gemini-2.5-flash`
- Split results view (NZC links + QAR questions)
- Copy to clipboard

## Run Locally

Open `index.html` in your browser.

For a local server (optional):

```powershell
cd .
python -m http.server 5500
```

Then open `http://localhost:5500`.

## Deploy to GitHub Pages

1. Create a new GitHub repository and push these files.
2. In GitHub, open **Settings > Pages**.
3. Set **Source** to **Deploy from a branch**.
4. Select branch **main** and folder **/(root)**.
5. Save and wait for deployment.

## Security Note

- API keys are stored in local browser storage on the current device only.
- Do not use a shared device without clearing the key after use.
