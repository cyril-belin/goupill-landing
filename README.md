# Goupill — landing page FR/EN

Public product landing for **Goupill** (Flutter personal AI assistant), built for the Devin for Startups application.

## Live website (GitHub Pages)

Publish the `main` branch at `/ (root)` under **Settings → Pages**. Once enabled, GitHub Pages serves:

https://cyril-belin.github.io/goupill-landing/

## Contents

- `index.html`: responsive bilingual landing (FR/EN), original Aube colors, high-contrast text, page navigation, and playable demo.
- `assets/omni-01.bin` … `assets/omni-18.bin`: the original Omni MP4 video stored as binary segments. The page fetches and reassembles them as a video Blob. This avoids issues uploading a single large media file through the repository connector; it does **not** change the video content.

## Checks

- Switch language using FR and EN controls.
- Click **Voir la démo / Watch the demo**, or use the video player to play, pause and adjust volume.
- The video requires a web server (GitHub Pages); opening `index.html` directly from the filesystem does not load the segments because browser `fetch()` disallows local-file cross-origin access.
- No store links or user signup are advertised during the private beta.

This repository contains only the public landing page, **not** Goupill's Flutter application or the older React Native codebase.
