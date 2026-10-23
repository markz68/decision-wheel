# Decision Wheel

A colorful, free, ad-free decision wheel Progressive Web App (PWA). Create multiple wheels (such as Dinner and Breakfast), add choices, and spin to select an option.

**App:** https://markz68.github.io/decision-wheel/  
**Current version:** 1.3.1

## Use

1. Select a wheel using **Choose wheel** beneath the spinner.
2. Press **SPIN!** to choose randomly from enabled choices.
3. Open **Manage Wheels** in the header to add, rename, or delete wheels, add/edit/remove choices, disable choices, **Bulk Add** one choice per line, or **Shuffle Choices**. Select **Done** to return to the spinner.
4. Review **Recent spins** on the main page. **Clear** clears the selected wheel's history after confirmation.
5. Open the **⚙️ gear icon** at the top right for Settings. It contains sound effects, **Export JSON**, and **Restore JSON**. There is no separate bottom Backup & Sync button.

Each enabled choice has an equal chance of winning a spin. Shuffle changes the visual order of choices, not their probability. The wheel uses sound effects when enabled.

## Install

- **Android (Chrome):** Open the app URL, then use the browser menu's **Install app** or **Add to Home screen** option when available.
- **Windows (Chrome or Edge):** Open the app URL and use the browser's **Install app** control/menu when offered.
- The app also works as a regular website. An internet connection is needed for the first load; previously cached assets support subsequent offline use.

## Data, backup, and privacy

Wheels, choices, and spin history are saved **locally in this browser/device**. They are not published to the GitHub repository and do not automatically appear on your other devices. Clearing browser/site data or removing the app may delete them.

To save your data, open the top-right **⚙️ Settings** gear and select **Export JSON**. Keep the downloaded backup somewhere safe. **Restore JSON** imports a previously exported backup and, after confirmation, **replaces the current local wheels and choices**. Export your current data before restoring another backup.

**Google Drive synchronization is not implemented** in Decision Wheel. Unlike some other PWAs, it does not currently offer cloud backup or cross-device sync.

## Updates and offline behavior

This app is hosted on GitHub Pages and uses a service worker to cache the app shell for offline use. Updates may require a refresh or reopening the installed PWA after the new version is published. The version appears in the app footer.

## Release notes

- **1.3.1:** Standardized the accessible top-right gear-only Settings button, refreshed offline cache, and documented installation, management, backups, and data storage.
- **1.3.0:** Moved wheel and choice management out of the main spinning view.
- **1.2.1:** Added Shuffle Choices.
- **1.2.0:** Added Bulk Add.

## Repository

Source: https://github.com/markz68/decision-wheel

The app uses `index.html`, `manifest.webmanifest`, `icon.svg`, and `sw.js`. When releasing a change, update the displayed app version, service-worker cache identifier, and this README when documented behavior changes.
