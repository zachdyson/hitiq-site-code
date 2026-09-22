# HITIQ site code

Hosted CSS/JS for the PROTEQT homepage on Webflow, served via jsDelivr.
Source of truth: `04 HIT IQ Site/v3-concept` (run `build/build.sh`, copy `dist/*` here, tag, push).

| File | Purpose |
|---|---|
| `hitiq.css` | Concept stylesheet (keyframes, sticky/parallax helpers, masks, reduced-motion). As Webflow classes take over, this shrinks to overrides only. |
| `hitiq.js` | Page behaviour: nav, reveal animations, impact chart, how-it-works cards, game-day sticky steps, timeline, gauge, rails, FAQ accordion, banner, footer. Needs GSAP + ScrollTrigger loaded first. |
| `hitiq-3d.js` | Hero mouthguard (three.js, ES module). |

Pin a tag in Webflow, never `@main`, so a push can't change the live site:
`https://cdn.jsdelivr.net/gh/<user>/hitiq-site-code@v0.1.0/hitiq.js`
