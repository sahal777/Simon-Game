# Simon Game

A simple Simon memory game built with HTML, CSS and JavaScript. Follow the flashing colors and sounds to repeat the sequence — the sequence grows by one color each level. This repository contains a lightweight, mobile-friendly implementation using jQuery for DOM interactions.

I created this README to help you add clear project documentation to your repo and explain how to run and customize the game.

---

## Demo

- Start the game by pressing any key.
- The game will show a sequence of colored pads; click the pads in the same order.
- If you make a mistake, a "Game Over" message and sound will play; press any key to restart.

---

## Features

- Classic Simon gameplay (repeat an ever-growing color sequence)
- Level indicator (Level X)
- Visual and audio feedback per button
- Keyboard start and mouse/touch support for the color buttons
- Simple, responsive UI with glowing neon style

---

## Built With

- HTML5
- CSS3
- JavaScript (ES5)
- jQuery (CDN link used in index.html)

---

## Project Structure

Recommended structure (your repo may already match):

- index.html
- style.css
- script.js
- /sounds
  - green.mp3
  - red.mp3
  - yellow.mp3
  - blue.mp3
  - wrong.mp3
- README.md

---

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari)
- Internet connection if you rely on the jQuery CDN; alternatively, download jQuery and update the script include.

### Run locally

Option 1 — Open directly:
1. Clone or download the repository.
2. Open `index.html` in your browser.

Option 2 — Serve with a simple HTTP server (recommended for consistent audio behavior):
- Using Python 3:
  - In the project folder run:
    - `python3 -m http.server 8000`
  - Open `http://localhost:8000` in your browser.
- Using Node (http-server):
  - Install: `npm i -g http-server`
  - Run: `http-server`
  - Open the printed local URL.

---

## Usage

- Press any key to start the game.
- Watch the sequence of flashes/sounds and click the colored pads in the same order.
- If you complete all steps for a level, you progress to the next level.
- On a wrong move, you'll hear a "wrong" sound, see a game-over visual, and the level resets.

---

## Customization

- Change colors, sizes, and layout in `style.css`.
- Modify game behavior (timing, difficulty, patterns) in `script.js`.
- Replace or add sound files in the `/sounds` folder (update names used by `playSound()`).

Tips:
- To make the UI more accessible, add focus states and ARIA attributes to the color buttons.
- To add keyboard keys for each pad, listen for `keydown` events and map keys to colors.

---

## Troubleshooting

- Audio won't play until the page receives a user interaction in some browsers — pressing a key or clicking the page will resolve this.
- If sounds fail to load, check that `/sounds/*.mp3` exist and file paths in `script.js` match.
- If the jQuery CDN is blocked, download jQuery locally and update the `<script>` tag.

---

## Contributing

Contributions are welcome. Suggested workflow:
1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`.
3. Commit your changes and push.
4. Open a pull request describing your changes.

Please open issues for bugs or feature requests.

---

## License

This project is provided under the MIT License. See LICENSE file for details (or add one if you want to publish with MIT).

---

## Credits

This project was originally inspired by a Simon Game tutorial from my course.
I studied the original version to understand the logic and then completely redesigned the layout, improved the styling, and wrote my own JavaScript logic to make it unique and beginner-friendly.

---
