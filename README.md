# My Build Track v3

This version fixes the branding/PWA deployment issues.

## Branding fixes
- Uses the supplied My Build Track logo in the sidebar.
- Uses the supplied logo in the top-right header instead of the MB circle.
- Includes a proper PWA manifest.
- Includes 180px Apple touch icon for iPhone Home Screen.
- Includes 192px and 512px PWA icons.
- Includes Apple mobile web app metadata.

## GitHub / Vercel update
Replace the contents of the root of the existing GitHub repository with:
- `index.html`
- `manifest.webmanifest`
- `assets/logo.jpeg`
- `assets/apple-touch-icon.png`
- `assets/icon-192.png`
- `assets/icon-512.png`

Do not upload the ZIP itself. Commit the files to the repository root. Vercel will redeploy automatically.

## iPhone
After Vercel redeploys, open the site in Safari. If the old icon is cached, remove the old Home Screen shortcut first, then use Share -> Add to Home Screen again. The new manifest/icon files will then be used.

## Data
The app continues to store data locally in the browser and supports JSON export/import.
