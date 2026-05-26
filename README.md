# 018 · Still Water

**Category:** G · Games and Interactive
**Live URL:** https://augustineiacopelli.github.io/appaday-018-still-water

---

## What It Does

Still Water is a meditative tap-to-explore experience. The screen shows a dark, living pond — subtle caustic shimmer lines breathe beneath the surface. Tap anywhere to cast ripples. Somewhere in the water, 8 hidden objects are waiting to be found. Land close enough to one and it surfaces with a glow, bobs gently, and is named on screen.

There is no timer. There is no fail state. There is only the water and the quiet satisfaction of discovery.

---

## How to Use

1. Open the app. Tap anywhere on the water to begin.
2. Watch for faint glowing pulses — they hint at something beneath.
3. Tap near a pulse to surface the hidden object.
4. Find all 8 to still the pond completely.
5. When the pond is still, tap **"still the water again"** to reset with a fresh set of 8 objects.

---

## Technical Notes

- Built with vanilla HTML, CSS, and Canvas 2D — no frameworks, no dependencies.
- Object pool contains 20 distinct hidden items; each session draws 8 at random, so no two ponds are identical.
- Ripple rings are drawn procedurally each frame with expanding radius and fading alpha.
- Undiscovered objects pulse with a radial gradient glow to remain findable without being obvious.
- Found objects drift and bob using a sine-wave offset applied per frame.
- Touch events handled with `passive: false` to prevent scroll interference on mobile.
- Fonts loaded from Google Fonts (Cormorant Garamond).

---

## Definition of Complete

- [x] Tap interaction creates visible ripple rings
- [x] 8 objects hidden per session, drawn randomly from a pool of 20
- [x] Object discovery triggers surface animation, glow, and name display
- [x] Found objects persist on screen with gentle drift animation
- [x] Reset button appears on full completion, starts a fresh session
- [x] Mobile-friendly — touch events, no horizontal scroll, tap targets adequate
- [x] No timer, no score, no fail state — purely meditative
- [x] Visually polished — deep water palette, Cormorant Garamond typography, cohesive aesthetic
