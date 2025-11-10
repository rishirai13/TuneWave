# 🎧 TuneWave

A sophisticated, minimalist web music player that delivers an exceptional listening experience through elegant design and smooth interactions.

## Overview

TuneWave is a modern music player built with vanilla web technologies, emphasizing clean aesthetics and intuitive functionality. The application provides essential playback controls, dynamic visualizations, and a responsive interface that adapts seamlessly across devices.

## Features

### Core Functionality
- **Playback Controls** — Play, pause, skip forward and backward through tracks
- **Progress Tracking** — Visual timeline with seek functionality
- **Volume Management** — Adjustable volume control with mute toggle
- **Playlist Navigation** — Browse and select tracks from your library

### User Experience
- **Responsive Design** — Optimized layouts for desktop, tablet, and mobile
- **Audio Visualization** — Real-time frequency display synchronized with playback
- **Smooth Animations** — Fluid transitions and micro-interactions
- **Keyboard Shortcuts** — Control playback without touching the mouse
- **Now Playing Display** — Album artwork, track title, and artist information

### Technical Highlights
- **Zero Dependencies** — Pure HTML5, CSS3, and JavaScript
- **Web Audio API** — Advanced audio processing capabilities
- **CSS Grid & Flexbox** — Modern, maintainable layout system
- **ES6+ JavaScript** — Clean, modular code architecture

## Technology Stack

```
Frontend:  HTML5, CSS3, JavaScript (ES6+)
Audio:     Web Audio API
Design:    CSS Grid, Flexbox, CSS Animations
```

## Getting Started

### Prerequisites
- Modern web browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- Local web server (optional, for testing)

### Installation

1. Clone the repository
```bash
git clone https://github.com/rishirai13/TuneWave.git
cd TuneWave
```

2. Launch the application
```bash
# Option 1: Direct file access
open index.html

# Option 2: Using Python's built-in server
python3 -m http.server 8000

# Option 3: Using Node.js http-server
npx http-server -p 8000
```

3. Navigate to `http://localhost:8000` in your browser

### Adding Music

Place your audio files in the `assets/music/` directory:

```
TuneWave/
├── assets/
│   ├── music/
│   │   ├── track-01.mp3
│   │   ├── track-02.mp3
│   │   └── track-03.mp3
│   └── covers/
│       ├── album-01.jpg
│       └── album-02.jpg
```

Update the playlist configuration in `js/playlist.js`:

```javascript
const playlist = [
  {
    title: "Midnight Dreams",
    artist: "Luna Wave",
    src: "assets/music/track-01.mp3",
    cover: "assets/covers/album-01.jpg"
  },
  // Add more tracks...
];
```

## Project Structure

```
TuneWave/
├── index.html              # Main HTML file
├── css/
│   ├── styles.css          # Core styles
│   ├── player.css          # Player component styles
│   └── animations.css      # Animation definitions
├── js/
│   ├── app.js              # Application initialization
│   ├── player.js           # Audio player logic
│   ├── visualizer.js       # Audio visualization
│   └── playlist.js         # Playlist management
├── assets/
│   ├── music/              # Audio files
│   ├── covers/             # Album artwork
│   └── icons/              # UI icons
└── README.md
```

## Usage

### Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Space` | Play / Pause |
| `→` | Next track |
| `←` | Previous track |
| `↑` | Volume up |
| `↓` | Volume down |
| `M` | Mute / Unmute |

### Controls

- **Play Button** — Click to play or pause the current track
- **Skip Buttons** — Navigate to the next or previous track
- **Progress Bar** — Click or drag to seek within the track
- **Volume Slider** — Adjust playback volume
- **Track List** — Click any track to start playing

## Customization

### Theming

Modify CSS variables in `css/styles.css`:

```css
:root {
  --primary-color: #1a1a1a;
  --accent-color: #6366f1;
  --text-color: #ffffff;
  --background: #0a0a0a;
  --card-background: rgba(255, 255, 255, 0.05);
}
```

### Visualizer Settings

Adjust visualization parameters in `js/visualizer.js`:

```javascript
const visualizerConfig = {
  barCount: 64,
  barWidth: 3,
  barGap: 2,
  smoothing: 0.8,
  minHeight: 2
};
```

## Browser Support

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 90+ | ✅ Fully Supported |
| Firefox | 88+ | ✅ Fully Supported |
| Safari | 14+ | ✅ Fully Supported |
| Edge | 90+ | ✅ Fully Supported |

## Performance

- **Lightweight** — ~50KB total bundle size (excluding audio files)
- **Fast Load** — Sub-second initial render
- **Smooth Animations** — 60fps playback and interactions
- **Efficient** — Minimal CPU usage during playback

## Contributing

Contributions are welcome. Please follow these guidelines:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/enhancement`)
3. Commit your changes (`git commit -m 'Add enhancement'`)
4. Push to the branch (`git push origin feature/enhancement`)
5. Open a Pull Request

### Code Standards
- Use ES6+ JavaScript features
- Follow consistent indentation (2 spaces)
- Comment complex logic
- Test across multiple browsers

## Roadmap

- [ ] Playlist creation and management
- [ ] Shuffle and repeat modes
- [ ] Equalizer with preset options
- [ ] Search and filter functionality
- [ ] Dark/light theme toggle
- [ ] Audio effects (reverb, echo)
- [ ] Integration with music APIs (Spotify, SoundCloud)
- [ ] Progressive Web App (PWA) support

## License

This project is licensed under the MIT License. See `LICENSE` file for details.

## Acknowledgments

- Design inspiration from modern music streaming platforms
- Audio visualization techniques adapted from Web Audio API documentation
- Icons provided by the open-source community

## Contact

**Project Maintainer:** Rishi Rai  
**Repository:** [github.com/rishirai13/TuneWave](https://github.com/rishirai13/TuneWave)

For questions, suggestions, or issues, please open an issue on GitHub.

---

Built with passion for music and clean code.
