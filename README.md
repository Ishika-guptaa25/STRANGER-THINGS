# Stranger Things - Cinematic Website

A cinematic frontend website inspired by the Stranger Things universe, built with pure HTML, CSS, and vanilla JavaScript

## DEMO
https://stranger-things-ochre.vercel.app/

## Screenshots
<img width="700" height="500" alt="image" src="https://github.com/user-attachments/assets/fd0e5840-7c83-41ad-a409-ea4d9c8dc644" />
<img width="700" height="500" alt="image" src="https://github.com/user-attachments/assets/05b116fa-1737-448d-9af6-85e8178d36e0" />
<img width="700" height="500" alt="image" src="https://github.com/user-attachments/assets/0dae3d57-cd08-4065-8efa-59bbdfcc4491" />
<img width="700" height="500" alt="image" src="https://github.com/user-attachments/assets/38cd768a-abc6-49fa-a4b9-bc064bd93e4c" />
<img width="700" height="500" alt="image" src="https://github.com/user-attachments/assets/ff80eefc-fc71-412b-89bc-d6c43aaec2a2" />

## Features

- Flickering neon title with letter-by-letter animation
- 3D depth effects using CSS perspective and transforms
- Parallax scrolling on all sections
- Animated particle system
- Interactive character cards with 3D tilt on hover
- Flashlight reveal effect in Upside Down section
- Vecna's Clock countdown timer
- Ambient audio system (Web Audio API)
- Glitch overlay effects
- Custom cursor with glow and flashlight
- Scroll-based reveal animations
- Fully responsive design

## Installation

### Method 1: Download
1. Download `index.html` from this repository
2. Open the file in your browser
3. No build process or dependencies required

### Method 2: Clone Repository
```bash
git clone https://github.com/Ishika-guptaa25/STRANGER-THINGS.git
cd STRANGER-THINGS
```
Then open `index.html` in your browser.

### Method 3: Run with Live Server
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx http-server

# Using PHP
php -S localhost:8000
```
Navigate to `http://localhost:8000`

## File Structure

Single HTML file containing:
- Embedded CSS styles
- Embedded JavaScript
- All functionality in one file

## Sections

1. **Hero** - Flickering title, particles, fog effects
2. **The Party** - Character cards with 3D hover effects
3. **The Upside Down** - Interactive flashlight reveal
4. **Vecna's Clock** - Live countdown timer
5. **Timeline** - Animated season milestones
6. **Footer** - Netflix-style credits

## Customization

### Change Doomsday Date
```javascript
// Line ~380 in JavaScript section
const DOOMSDAY = new Date('2026-07-04T00:00:00').getTime();
```

### Adjust Particle Count
```javascript
// Line ~230 in createParticles() function
for (let i = 0; i < 30; i++) {
```

### Modify Colors
```css
/* Primary red color used throughout */
--primary: #ff0000;
--dark-red: #8b0000;
```

### Audio Settings
```javascript
// Line ~170 in playEerieAmbience() function
osc1.frequency.setValueAtTime(40, audioCtx.currentTime);  // Deep rumble
gain1.gain.setValueAtTime(0.03, audioCtx.currentTime);    // Volume
```

## Browser Compatibility

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Requires JavaScript enabled
- Web Audio API support needed for sound

## Performance Optimizations

- Mobile particle count automatically reduced
- RequestAnimationFrame for smooth animations
- Intersection Observer for scroll animations
- CSS transforms for hardware acceleration
- Conditional cursor effects

## Key Technologies

- HTML5
- CSS3 (Animations, Transforms, Gradients)
- Vanilla JavaScript (ES6+)
- Web Audio API
- Intersection Observer API
- RequestAnimationFrame

## Usage

1. Open `index.html` in a modern browser
2. Click "SOUND: OFF" button to enable ambient audio
3. Move mouse to see parallax and flashlight effects
4. Scroll to reveal animated sections
5. Hover over character cards for 3D tilt

## Important Notes

- Single file - no external dependencies
- No frameworks or libraries required
- Custom cursor replaces default cursor
- Audio requires user interaction to start
- Flashlight effect most visible in Upside Down section
