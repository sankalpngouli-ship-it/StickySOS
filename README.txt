# StickySOS PWA

This package converts the existing StickySOS HTML app into a Progressive Web App without Android Studio.

## Files
- `index.html` — StickySOS app
- `manifest.json` — install/app metadata
- `service-worker.js` — app-shell caching and update handling
- `icons/` — recreated vector StickySOS logo rendered as PWA icons

## Important
Host the folder on HTTPS (or localhost for development). Do not open `index.html` directly with `file://`; service workers require a secure context.

## Publish to Android without Android Studio
1. Upload this folder to an HTTPS web host.
2. Open PWABuilder and enter the public HTTPS URL.
3. Fix any report-card items it flags, if any.
4. Choose Android and generate the package.
5. Test the generated Android package on a real phone before Play Store submission.

The current HTML still loads QR generation and camera-scanning libraries from their CDNs, so the first PWA version should be tested online.
