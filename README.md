# BB Pose Alterations Creator

Internal tool for generating 4 pose variations of a winning ad creative and uploading them to the All Creatives folder in Google Drive.

## How it works

1. Team opens the URL (shared privately)
2. Uploads a creative, types product name + color
3. Backend (n8n workflow) generates 4 variations and uploads to Drive
4. Takes about 90 seconds

## Files

- `index.html` — the form page
- `logo.png` — BB shield logo

## Deploy (GitHub Pages)

1. Push this folder to a GitHub repo
2. Repo Settings → Pages → Source: `main` branch, `/` root
3. Wait ~1 min, URL will be `https://<username>.github.io/<repo>/`

## Backend

Submits to n8n production webhook:
`https://bb-boutique-enterprises.app.n8n.cloud/form/b.b.pose.alterations`

Workflow: "Creative Pose Alterations" (ID: sX1HUcj1DRQkJ2Gm)
