# Snake

A single-file Snake game. Open `snake.html` in a modern web browser to play.

## Changes

- Added a start menu with difficulty selection and a locally saved top-five leaderboard for each difficulty.
- Added smooth interpolated snake movement, an eating particle burst, and a floating `+1` score effect.
- Added a coordinated CSS-variable color palette with high-contrast overrides.
- Added synthesized eat, pause, and game-over sounds, with a saved mute toggle.
- Added a pause menu with Resume, Restart, and Main menu actions.
- Improved turn buffering, tail collision handling, food placement, full-board wins, and pause/resume timing.
- Added visible keyboard focus, live score and end-of-game announcements, 44px minimum button targets, responsive layout rules, and reduced-motion support.
- Checked text color pairs against WCAG AA contrast thresholds. `git diff --check` reported no whitespace errors.

## Notes and limitations

- The game has not been run through browser or screen-reader testing. The responsive layout and live announcements still need hands-on verification.
- Contrast ratios were calculated from the configured colors; translucent overlays and browser-rendered colors were not sampled.
- Sound requires browser Web Audio support and may require a user gesture to start. Settings and leaderboard scores use local storage, which can be unavailable or cleared.
- The game uses modern browser features such as Canvas `roundRect`, `matchMedia`, and CSS `backdrop-filter`; older browsers may render it differently.
