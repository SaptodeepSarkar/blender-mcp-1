# Car Showdown — 60s Studio Reveal (Storyboard)

**Car:** Toyota Supra Mk4 (real model) · **Room:** black studio void · **Cover:** red leather, cloth-sim pull-off
**Light:** top softbox slam-on · **Cameras:** 3 rigs, 7 shots · **Format:** 1280×720, 24fps, 1440 frames
**Engine:** Cycles GPU (OptiX, 128 samples + denoise)

## Story arc

Dark → cover rip-off → headlights ignite → hero showcase → **car takes off** (launches forward out of frame).

## Shot list (camera bindings = timeline markers)

| # | Frames | Time | Camera | Move | Story beat |
|---|--------|------|--------|------|------------|
| 1 | 1–199 | 0.0–8.3s | Camera1 (orbit, 40mm) | Slow push-in arc, low angle | **Dark.** Top light slams on ~f110. Red leather cover silhouette over the car |
| 2 | 200–429 | 8.3–17.9s | Camera2 (dolly, 55mm) | Lateral track left→right | **Reveal.** Wind + hook rip the cover off (+X). Stock headlight bars ignite ~f290–330 |
| 3 | 430–699 | 17.9–29.1s | Camera1 (orbit, 40mm) | Continued orbit, car fully exposed | **Showcase I.** Stock lenses glowing, paint + rims catch top + blue/orange rims |
| 4 | 700–939 | 29.1–39.1s | Camera3 (crane, 35mm) | High → swooping low | **Showcase II.** Glasshouse detail (transparent glass, lit cabin) → low aggressive nose |
| 5 | 940–1139 | 39.1–47.5s | Camera2 (dolly, 55mm) | Slow push, shallow feel | **Showcase III.** Side profile glide. Wheels + skirt + wing line |
| 6 | 1140–1299 | 47.5–54.1s | Camera3 (crane, 35mm) | Low rear drift | **Tension.** Rear 3/4. Wing silhouette against black, red rim-light pool. Engine-rev hold |
| 7 | 1300–1440 | 54.1–60s | Camera1 (orbit, 40mm) | Hold as car exits | **Takeoff.** Supra launches forward −Y, 26m over 140f, exits frame. Top light pulses 6000→4000. End on empty black studio + light trails |

## Key event frames

- f1: black, top energy 60 · f110: top → 4000 (slam) · f180–460: wind 0→3200→0, hook drags cover +X (cloth cache 1–560)
- f290–330: stock headlight-bar emission 0 → 15 (model's own materials, no add-on geometry) · f1300: car at rest (marker) · f1440: car −26m Y (gone)
- f1330: top pulse 6000 · f1400: settle 4000

## Composition rules (every shot)

1. Car sits on lower-third line, never center-frame (shots 1–3, 5, 7); detail shots (4, 6) put badge/light on third-intersections.
2. Nose room: twice as much space ahead of the car as behind in direction of implied motion (critical in shot 7 — exit side stays open).
3. 180° rule: all cameras stay on the orbit's front hemisphere between cuts — no side flips.
4. Lens logic: 55mm dolly = compressed profile/side, 40mm orbit = hero depth, 35mm crane = sweeping context.
5. Light logic: top softbox = key/shape, blue rim (camera-left) vs orange rim (camera-right) = showdown contrast. Headlights = practicals + floor pools.
6. Cover must fully exit frame by f500 — no cloth in hero shots. Car must fully exit frame by f1440 — end on void.

## Sources (all free)

- Supra model: GitHub `grimdeathr/models` (`supra.glb`, 12MB)
- HDRI: Poly Haven `studio_small_09_1k` (CC0, reflections only)
- Floor: Poly Haven `asphalt_02` 1k (CC0, darkened 0.35×)
- Cloth: Poly Haven `leather_red_02` 1k (CC0)
