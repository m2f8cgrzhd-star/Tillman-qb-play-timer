# Tillman QB Play Timer

A mobile-first, installable web timer for quarterback training. Core features are designed to run client-side with local preset storage and no backend or subscription.

## Current MVP features

- Internal-clock mode with 1–10 second duration, per-second short beep, final buzzer
- Read-progression mode with four independently enabled cues adjustable to hundredths
- Immediate, delayed (3/5/7/10 seconds), and experimental voice trigger start
- Optional spoken countdown during solo delayed start
- Preview tone and volume control
- Pause/resume/reset
- Save/load/rename/delete local presets
- Export/import preset backup JSON
- PWA manifest and offline service worker

## Deploy with GitHub Pages

1. Repository Settings → Pages.
2. Under Build and deployment, choose **Deploy from a branch**.
3. Select branch `main`, folder `/ (root)`, and Save.
4. Wait for deployment. The site URL will be `https://m2f8cgrzhd-star.github.io/Tillman-qb-play-timer/`.

GitHub Pages may take several minutes to publish after setup or a commit.

## Important testing notes

- Voice cadence recognition is experimental and browser-dependent. Speech recognition may be delayed, unavailable, or handled by a remote service. Do not use it as the only start option.
- Web audio requires a user gesture to initialize. The first tap on Start or Preview should enable audio.
- Presets are local to each browser/device. Export/import is the transfer method.
- On iPhone, after deployment, open the URL in Safari → Share → Add to Home Screen. Load it once while online for offline cache.
- Keep public repository and app source free of private personal information.
