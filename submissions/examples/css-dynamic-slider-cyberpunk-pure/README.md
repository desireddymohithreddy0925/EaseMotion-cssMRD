# Cyberpunk Dynamic Slider

A purely HTML/CSS dynamic range slider with a striking Cyberpunk aesthetic.

## Features
- **Pure HTML/CSS**: No JavaScript is required for the styling, hover effects, or active states.
- **Cyberpunk Aesthetics**: Features neon colors (cyan, magenta, yellow), clipped corners (using `clip-path`), grid background, and stark contrast.
- **Glitch Effects**: Hovering over the container triggers a CSS text glitch animation. A static glitch overlay adds texture to the container.
- **Custom Input Range**: Completely overhauls the default browser `<input type="range">` using vendor prefixes (`::-webkit-slider-thumb`, `::-moz-range-thumb`, etc.) to match the cyberpunk style.
- **Responsive**: Adapts to smaller screen sizes automatically.
- **Accessibility**: Includes `prefers-reduced-motion` to stop pulsing animations and glitch effects for users who prefer it. Focus states are clearly defined with an outline.

## Usage
Simply open `demo.html` in your browser. Interact with the slider to see the thumb's hover and active state transformations.

## Files
- `demo.html`: The HTML structure of the slider and decorative elements.
- `style.css`: All the CSS styling, variables, animations, and cross-browser input range resets.
