# Date Maker — Interactive Web Experiment

**Status: small static HTML/JavaScript experiment.**

[Live page](https://cianium.github.io/Date-maker/) · [Source](https://github.com/cianium/Date-maker)

A playful, single-page invitation experience made with HTML, CSS and JavaScript, featuring animated buttons and visual responses to user choices. It is a front-end experiment, **not** a booking or calendar service.

## Run locally

```bash
python3 -m http.server 8080
```

Open `http://localhost:8080`. No package manager or external build step is present in the current repository.

## Repository contents

- `index.html` — page UI, styling and client-side interactions
- `Spongi.jpg` — image asset
- `radiohead_-_jigsaw_falling_into_place.mp3` — audio asset

## Limitations and improvement ideas

- No automated tests, CI or user-data backend
- Add semantic controls, reduced-motion handling and keyboard support
- Improve mobile viewport behavior and check browser autoplay restrictions
- Move assets/styles/scripts into maintainable folders if the experiment expands

## Copyright and distribution

**Important:** publishing an MP3 or image in a public repository does not grant permission to redistribute it. Confirm rights to the included song and image; remove or replace media that you are not licensed to distribute. No software license is declared for this repository.
