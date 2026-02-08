# Playables (HTML5)

This repository contains **HTML5 playable creatives** used for marketing our apps.

## Structure

* **PB/**: Playables for PB.
* **TS/**: Playables for TS.

Inside each app folder, playables are organized by **variant**.

## Variant layout

Each variant includes two entry points:

* **test.html**: A device preview version for local testing, to see how the playable looks on a phone sized frame.
* **index.html**: The production version used for packaging and uploading to ad networks.

## Rules

* **HTML5 only**
* Keep everything **self contained** (no external CDNs, fonts, or remote assets).
* Optimize for **fast load** and **mobile WebView** compatibility.

## Local testing

You can open `test.html` directly, or run a simple local server:

* `python3 -m http.server 8080`
* Open `http://localhost:8080` and navigate to the desired variant folder.

## QA checklist

* Works on common mobile screen sizes
* No console errors
* Interactions feel responsive
* `index.html` has no debug UI that is only meant for `test.html`
* Asset sizes are reasonable (compress images, avoid heavy audio)
