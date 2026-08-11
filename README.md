# UP Roadways

A single-page immersive web experience inspired by Uttar Pradesh highway travel. The site recreates a nostalgic bus journey with animated scenery, a playable 90s Bollywood "Highway Radio" music player, and a stylized UP Roadways bus illustration.

## Overview

This project is a lightweight HTML/CSS/JavaScript landing page designed to look and feel like a vintage UPSRTC highway radio experience. It uses a fullscreen SVG scene, custom animated elements, and a simple audio player UI.

## Key Features

- Fullscreen responsive scene built with SVG and CSS
- Animated bus, road, clouds, and scenery motion when playback is active
- Floating glassmorphic player bar with vinyl disc and track metadata
- 20-track 90s Bollywood playlist with next/previous controls
- Keyboard-friendly controls using buttons and accessible ARIA labels
- Horn button that generates a short synthesized horn sound using Web Audio
- Live clock display and animated track playlist panel
- Responsive layout for mobile and desktop
- Reduced-motion support via `prefers-reduced-motion`

## Project Structure

- `index.html` — single HTML file containing the full UI, inline styles, SVG artwork, playlist logic, and playback behavior.
- `README.md` — project documentation and usage details.

## Design Notes

- The scene is rendered entirely in SVG with gradients, path shapes, and grouped scenery layers.
- A top header displays the current local time and a playlist toggle button.
- The bus illustration includes UPSRTC-inspired branding, window reflections, wheels, and a realistic-style body.
- The bottom player uses a vinyl motif and animated seek bar to suggest an audio playback interface.
- The playlist drawer slides in from the right with track metadata and active track highlighting.

## How to Use

1. Open `index.html` in a modern browser.
2. Click the central play button to start the audio playback.
3. Use the previous and next buttons to navigate between tracks.
4. Click the top-right playlist button to open or close the track list.
5. Tap the horn button to play a short horn sound.
6. Drag or click on the seek bar to jump within the current track.

## Technologies

- HTML5
- CSS3
- SVG graphics
- JavaScript
- Web Audio API

## Accessibility

- Buttons include `aria-label` attributes for screen readers.
- The playlist panel uses `role="listbox"` and each track item uses `role="option"`.
- Motion is reduced automatically if the user prefers reduced motion.

## Notes

- Audio playback relies on remote MP3 URLs. For offline use, replace the `actualAudioUrls` array in `index.html` with local audio assets.
- The current implementation uses a static playlist and does not include server-side logic.
- The page should work in modern browsers that support SVG, HTML5 audio, and Web Audio API.

## License

Use this project freely as a demo or inspiration for interactive travel-themed landing pages.
