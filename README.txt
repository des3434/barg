# Barg Continental - PWA Export

## How to create a standalone app (no browser chrome):
1. Host these files on any web server (Netlify, Vercel, GitHub Pages, etc.)
2. Visit your hosted URL
3. Go to https://pwabuilder.com
4. Enter your hosted URL
5. IMPORTANT: Under "Android Package Options", select "Other Android" (NOT "Google Play")
   - This creates a proper TWA that runs without the browser address bar
6. Download and sign the APK

## Files included:
- index.html - The menu app
- manifest.json - PWA manifest (configured for standalone mode)
- sw.js - Service worker for offline support
- icon-192.png - App icon (192x192)
- icon-512.png - App icon (512x512)
- icon-maskable-192.png - Maskable icon (192x192)
- icon-maskable-512.png - Maskable icon (512x512)
- screenshot.png - App screenshot
- project.json - Backup of your project data

## Troubleshooting:
If the app still shows browser chrome after installation:
1. Make sure you selected "Other Android" in PWABuilder, not "Google Play"
2. Clear the app data and reinstall
3. Ensure the manifest.json display is set to "standalone"
