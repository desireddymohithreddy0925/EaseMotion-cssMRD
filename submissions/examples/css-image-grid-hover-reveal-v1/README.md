# CSS Reveal on Hover Grid

A responsive image gallery that elegantly reveals information overlays and quick actions entirely on hover, built without JavaScript.

## Features
- Pure CSS and HTML (Zero JavaScript required for hover state detection or grid responsiveness).
- **Theming & Dark Mode**: Utilizes CSS Custom Properties (`--overlay-bg`, `--accent`, etc.) for easy overriding. Automatically respects the OS-level system theme (`prefers-color-scheme: dark`).
- **Responsive CSS Grid Architecture**: The `.image-grid` container uses `grid-template-columns: repeat(auto-fill, minmax(280px, 1fr))` to automatically wrap and scale cards across any screen size without relying on media queries.
- **Staggered Hover Reveal Animation (Documented in Code)**: 
- The hidden overlay (`.item-overlay`) starts with `opacity: 0` and is brought into view using the `.grid-item:hover .item-overlay` selector.
- The inner content (`.overlay-content` and `.overlay-actions`) are initially pushed down using `transform: translateY(20px)` and `translateY(30px)`.
- When hovered, they slide up to `transform: translateY(0)` with slight `transition-delay` values (0.05s and 0.1s). This creates a polished, staggered entrance effect.
- The underlying image (`.item-image`) also scales up slightly to create depth.
- **Accessibility**: Includes `:focus-visible` pseudo-class support so the overlays reveal for keyboard users navigating via the `Tab` key. Fully supports `prefers-reduced-motion` to disable sliding/scaling for motion-sensitive users.

## Usage
Open `demo.html` in your browser. Hover your mouse over any image card (or focus via keyboard) to see the glassmorphism overlay fade in and the content slide up.

## Files
- `demo.html`: The HTML structure detailing the image grid.
- `style.css`: The styling, CSS Custom Property theming blocks, and heavily commented mechanics detailing the CSS Grid and Hover Transform logic.
