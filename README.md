#f6978d — Cutlery Concept Landing

Open `index.html` in a browser to view the landing page.

What this has:
- Rotating circular text created with SVG `textPath` around a circle.
- A circular center "buy now" button in the requested color `#f6978d` with white text.

Fonts:
- The repository includes the variable TTF at `Assets/DarkerGrotesque-VariableFont_wght.ttf` and the stylesheet embeds it via @font-face so the page will use it automatically.

Fitting text to the circle:
- A small inline script in `index.html` measures the circle path length and sets `textLength` and `lengthAdjust="spacingAndGlyphs"` on the SVG textPath so the sentence fills the circle without a gap. It also adjusts font-size slightly based on the path length and recalculates on window resize.

Customization:
- Change `--accent` or `--accent-dark` in `styles.css` to tweak the colors.
- Adjust rotation speed in the `@keyframes spin` animation.

Project page:
- Clicking the "buy now" button opens `project.html`. This page uses `Assets/Circles tile.png` as a repeating background and pans the background in the same direction as your cursor movement to create an infinite-space tiling effect. Click-and-drag for stronger motion.
