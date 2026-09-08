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


## v3.5 Bode Analysis
Added Bode analysis engine notes and frequency-response framework.


## v3.6 Nyquist Analysis
- Added Nyquist analysis documentation and framework planning.

## v3.7 State Feedback Control
- Added state feedback control design framework
- Added controllability and observability workflow
- Added pole placement design notes


## v3.8 Observer Design & State Estimation
- Added observer design planning notes
- Added state estimation framework roadmap
