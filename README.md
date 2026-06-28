# My Ride — Mobile App

Mobile companion for the My Ride cycling training log desktop app.

**Live app:** https://moriteuk.github.io/RideApp/

## How it works

Signs in with your Microsoft account (the same one used for Outlook in the desktop app), then reads and writes data from `#Personal/Cycling/myride-data.json` in your OneDrive — kept in sync with the desktop app automatically.

## Azure setup (one-time)

1. Go to [portal.azure.com](https://portal.azure.com) → Azure Active Directory → App registrations
2. Find app `726ecfd2-1b76-499b-9ef4-3dbd26a18097`
3. Click **Authentication** → **Add a platform** → **Single-page application (SPA)**
4. Add redirect URI: `https://moriteuk.github.io/RideApp/`
5. Save

## Installing on Android (Pixel 8)

1. Open Chrome, go to https://moriteuk.github.io/RideApp/
2. Tap the Chrome menu (⋮) → **Add to Home screen**
3. Sign in with your Microsoft account

## Updating

Any push to this repo automatically redeploys via GitHub Actions.
To update the app code, copy the latest `index.html` from the desktop app's `mobile-app/` folder into this repo and push.
