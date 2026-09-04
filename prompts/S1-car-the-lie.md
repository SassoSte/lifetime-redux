# S1 — The Car (Scene 1, 0:00–0:12)

**Shot:** single full-scene generation, no sub-shots.
**Attach from `redux/refs/`, in this order:**

| Slot | File |
|---|---|
| `@[Image 1](image_1)` | `Seth-Car.png` |
| `@[Image 2](image_2)` | `Lifetime-Fitness-Exterior.jpeg` |

**What this shot has to deliver that the original did not:** the *"oh shit, here we go"*
look-up at camera. He is typing, looking down, and then he looks straight up the lens —
at us — with the flat expression of a man who knows exactly what he is about to do. Not
a smirk, not a wink. That look is the setup for the entire series.

**The failure this prompt is built to avoid:** the original render put the phone screen
and his hands in frame and produced gibberish text and mangled fingers. The fix is
staging, not prompting — the phone and both hands stay **below the frame line** for the
whole take. He is a face and a pair of shoulders. The typing is read entirely off his
eyes, his jaw and the small movement in his upper arms.

---

## THE PROMPT

```
Seth sits in his parked car, bemused, outside a health club at golden hour and types a
text to his wife that is not quite true — a glance up at the building, thumbs working
below frame, one flat knowing look straight down the lens, and the send.

The shot lives inside @[Image 2](image_2) exactly, seen from inside a parked car: a
modern multi-story fitness club across a late-afternoon parking lot, pale stone and
reflective glass, a central stone tower, a dark awning over the entrance, palms and
low desert shrubs, all of it soft and slightly out of focus through the windshield
beyond him. The interior is an ordinary, well-kept, unpretentious American car — grey
cloth seats with visible weave and creasing, a plain dark dashboard, a headrest, a
seatbelt across his chest. Real Scottsdale golden-hour sun comes through the windshield
from front-left, warm edge-light along his cheekbone, the bridge of his glasses and his
shoulder; soft skylight fill through the side window; the cabin falls away to gentle
shadow behind him. Fine natural grain, no glow, no bloom, no lens flare. A pair of
sunglasses and a set of keys sit in the console tray, untouched.

Seth is @[Image 1](image_1) exactly: early forties, slender untrained build with a soft
midsection, dark brown hair cut short at the sides and tousled on top, clearly receding at
the temples and thinning at the crown, a high lined forehead, a short patchy reddish-brown
stubble beard with a few greys at the chin, black rectangular eyeglasses with clear
unfogged lenses, matte organic skin with visible pores and
natural asymmetry, wet living eyes with warm catchlights. He wears a heather-grey polo
with a pen in the placket and a seatbelt across it. Nothing in his visible hands —
his hands and the phone stay entirely below the bottom of the frame for the whole
shot, never rising into view, and no screen, no glow and no reflected light from a
screen ever appears anywhere in the frame or on his face.

One continuous static shot, 0s to 12s — medium close-up, chest-up, eye level, 50mm,
shot from the passenger seat looking across at him, the frame identical at the end to
the first pixel. He sits in the driver's seat on the left, frame-center, the steering
wheel a soft dark curve in the near foreground at the bottom-left edge, the club
building small and soft through the windshield behind his right shoulder. He looks up
and out through the windshield at the building for a beat, unhurried, the way you look
at a restaurant you are early for. He lowers his eyes to his lap — below frame — and
his jaw sets very slightly as his upper arms make the small contained movement of a man
typing with two thumbs; his eyes track a line of text he is composing, left to right,
twice. He stops. Then he raises his head and looks straight down the lens, directly at
camera, and holds it — a flat, unembarrassed, wholly knowing look, held a full beat too
long, the look of a man who has already decided. His eyes drop once more, one thumb
movement, and he exhales; a tiny private almost-smile arrives at one corner of his
mouth and does not become a grin. He settles back into the headrest and the frame holds.

Camera law: locked-off tripod, 50mm prime, eye level, absolute rock-solid stillness from
first frame to last — zero drift, zero shake, zero stabilization float, zero pan, tilt,
zoom, dolly or breathing. The clip closes on precisely the framing it began with.

Warm natural golden-hour grade, documentary realism, gentle highlight roll-off on the
windshield, fine film grain, no stylization and no teal-orange push. Audio: diegetic
ambient only — cabin hush, the low tick of a cooling engine, distant parking-lot traffic,
faint air-conditioning fan, two soft fingertip taps, one shallow breath and one exhale.
No music, no score, no bgm.

Count of people in frame: one. Count of phone screens visible in frame: zero. Count of
hands visible in frame: zero — hands stay below the frame line throughout. Count of
readable words, letters or digits anywhere in frame: zero. Count of camera moves: zero.
Count of smirks, winks or eyebrow raises during the look at camera: zero — the look is
flat and knowing. Every expression reads as warm amusement at his own theatrics, never
grim, never guilty, never heroic.
```

---

## Verification checklist

Extract frames at 2s, 5s, 7s, 9s, 11s.

| # | Check | Pass |
|---|---|---|
| 1 | Hands and phone never enter frame; no screen glow on his face | ☐ |
| 2 | Zero readable text anywhere — dash, building signage, windshield | ☐ |
| 3 | The look-to-camera happens, is held, and is **flat** — not a smirk or a wink | ☐ |
| 4 | Face matches `Seth-Car.png` — glasses, beard, hairline | ☐ |
| 5 | Skin matte with visible pores, not waxy | ☐ |
| 6 | Golden-hour light is directional and warm, not a uniform glow | ☐ |
| 7 | Camera dead static, first frame = last frame | ☐ |
| 8 | Register is bemused/knowing, never guilty or grim | ☐ |

**Pass threshold:** 6/8, with checks 1, 2 and 3 mandatory. Failing 3 means re-run;
failing 1 or 2 means the phone staging leaked and must be re-run.

**Save as:** `redux/outputs/S1-v1.mp4`
