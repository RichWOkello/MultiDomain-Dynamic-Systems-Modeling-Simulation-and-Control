# Stability Demonstration Update

Replace only `docs/app.js` on the `website-development` branch.

New behavior:
- Mechanical damping can be negative.
- Electrical resistance can be negative.
- Pneumatic and hydraulic damping can be negative.
- Stable, marginal and unstable states are classified live.
- Pole locations are displayed.
- Unstable responses turn red and show `DIVERGING RESPONSE`.
- Marginal responses use amber.
- Runaway values are bounded so the browser plot remains usable.
