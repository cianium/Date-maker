<div align="center">

# Date-maker

### Interactive Static Web Experiment

**HTML · CSS · Vanilla JavaScript · GitHub Pages**

[Live Demo](https://cianium.github.io/Date-maker/) · [Source Code](https://github.com/cianium/Date-maker) · [Release Audit](RELEASES.md)

</div>

> **Status:** A small interactive front-end experiment, **not** a calendar, scheduling, booking or messaging service. The site displays a question and playful buttons, an image and background audio. No server, login, database or calendar integration exists in this repository.

## Overview

Date-maker is a single-page interactive website. All layout, styles and JavaScript logic are embedded in `index.html`.

The page responds to visitor button interactions, can display a popup, starts local audio after a browser interaction (subject to the browser's playback policy) and can attempt to open the native SMS composer.

This is a **static browser experience**, not a service that makes an appointment or sends messages automatically.

## Included files

```text
Date-maker/
├── index.html                        HTML, CSS, interactions and SMS launcher
├── Spongi.jpg                        Image displayed in the page
├── radiohead_-_jigsaw_falling_into_place.mp3
│                                     Background audio — rights not verified
├── README.md                         Overview, setup and limitations
└── RELEASES.md                       GitHub tag and release history audit
```

There is no `package.json`, `node_modules`, backend, automated test suite or build configuration.

## Run locally

```bash
git clone https://github.com/cianium/Date-maker.git
cd Date-maker
python3 -m http.server 8080
```

Then visit **http://localhost:8080/**.

Python is used only as a lightweight static file server. The page itself uses HTML, CSS and vanilla JavaScript; no dependency installation is required.

## What the current code does

- Shows a fixed-layout question screen with two buttons.
- Moves one button in response to pointer/touch interactions and may open an image modal.
- Starts an audio element after a user interaction when the browser permits playback.
- Uses an `sms:` URL to ask the user's device to open its messaging application after a specific button interaction.
- Does not collect form submissions, save user data in a database or integrate with calendar providers.

### SMS and privacy

**The current `main` branch no longer embeds a specific recipient phone number in its SMS launcher.** It opens the `sms:` scheme without a predefined recipient; the user must choose a destination and confirm sending in the native messaging app. Desktop browsers or mobile devices without an SMS handler may not support this operation.

**Historical warning:** Older Git commits, the `v1.0`/`v1.2` tags and externally uploaded release ZIPs may still include a formerly hard-coded phone number. Editing the latest `index.html` does **not** erase Git history, external archives, caches or clones. Review historical copies before sharing or distributing them.

## Limitations and improvements

- **Accessibility:** The moving-button interaction can be difficult or impossible for keyboard, assistive technology and some touch users. Evaluate an interaction that respects an ordinary decline, and support visible keyboard focus and accessible modal dismissal.
- **Responsive behavior:** Fixed viewport sizing and absolute button placement may be unreliable on very narrow or landscape screens. Test different screen sizes and zoom levels.
- **Motion and sound:** Honor `prefers-reduced-motion`, provide a clear audio pause/mute option and avoid relying on autoplay.
- **Privacy:** Do not reintroduce actual phone numbers, personal communications or private content in public source files.
- **Testing:** Add simple browser checks for button actions, viewport boundaries, keyboard focus, modal state and SMS-fallback behavior.

## Deployment

The repository is published through GitHub Pages at:

**https://cianium.github.io/Date-maker/**

[GitHub Pages build history](https://github.com/cianium/Date-maker/actions) includes successful deployments. Deployment success is **not** proof that every feature works in current mobile browsers.

## Release status

Two historical GitHub pre-releases exist:

- [`v1.0`](https://github.com/cianium/Date-maker/releases/tag/v1.0)
- [`v1.2`](https://github.com/cianium/Date-maker/releases/tag/v1.2)

**Both version tags reference exactly the same Git commit.** Neither release includes an official attached Release Asset; the descriptions instead link to externally uploaded ZIP files whose correspondence with the tags is unverified.

The latest `main` branch contains subsequent documentation and privacy changes and is not equivalent to either historical pre-release. Consult [RELEASES.md](RELEASES.md) for verified details and suggested description corrections. No new release is implied by this README update.

## Copyright and licensing

The included MP3 appears to be a commercial music recording; **the right to publish or redistribute it has not been verified**. Check and obtain permission or replace/remove it before public distribution. The image's rights are also unverified.

No separate repository-wide software license was found. Public visibility does not itself grant redistribution permission.

---

<div align="center">

**Date-maker — a small client-side interaction experiment.**

</div>
