# S4 — Sauna Psych-Up (Scene 4, 0:36–0:48) — **LOCKED KEEPER**

**Do not re-generate.** This shot already exists and scored 8.5/9:
`higgsfield-supercomputer/scene-4-attempt-3-external-2026-09-03.mp4`
(md5 `9dc89a8fa37739bb15e7cc04e4051fa2`, identical to `~/Downloads/hf-man-in-sauna.mp4`).

It is recorded here because it is **the canonical shape** — every other redux prompt is
written to match it. If a later prompt is failing, diff it against this one.

**Attach from `redux/refs/`:**

| Slot | File |
|---|---|
| `@[Image 1](image_1)` | `Seth-Swim-Bare.png` (was `Man-Swim-v2.png` — see note below) |
| `@[Image 2](image_2)` | `Sauna-Interior.png` |

---

## THE PROMPT (as sent, verbatim)

```
Seth steels himself, bemused, in a hot sauna for the cold plunge waiting beyond the glass
door — breath work, streaming sweat, a small private smile, and one slow reach for the
handle.

The shot lives inside @[Image 2](image_2) exactly: a modern cedar sauna with horizontal
plank walls and ceiling, natural grain variation, visible knots and imperfect joints, a
two-tier built-in bench, a stone-clad corner with a cedar heater full of glowing
orange-red stones, and a black-framed glass door on the right leading to the plunge room.
Warm recessed strip lights along the cedar cast a soft amber glow; the air is thick and
humid with visible moisture haze, heat shimmer rising off the stones in visible waves,
white wisps of steam curling upward. Folded white towels and a water bottle sit
undisturbed on the far end of the bench.

Seth is @[Image 1](image_1) exactly: early forties, thin build with a slightly soft
midsection, dark brown neatly trimmed hair, light stubble, matte organic skin with
visible pores and natural asymmetry. His face is completely bare — his eyes are
uncovered, pale and slightly asymmetrical, wet and living with amber catchlights. He is
shirtless in plain navy-blue swim trunks, barefoot. Nothing on his face, nothing draped
over his shoulder, nothing in his hands. His skin glistens wet with sweat under the amber
light, droplets streaming down his brow, neck, chest and arms.

One continuous static shot, 0s to 12s — medium shot, waist-up, eye level, 35mm, the frame
identical at the end to the first pixel. He sits on the LOWER bench, frame-center, body
facing slightly left, the glowing heater deep in the background right, the glass door at
far right. Eyes closed, he does slow breath work, chest rising and falling, sweat
streaming down his forehead and catching the light; a bead drips from his chin onto his
chest and he does not wipe it. He opens his eyes, turns his hands over and studies the
sweat glistening on his palms, a small bemused "hmm", then wipes his brow with the back
of his hand, slow and unhurried, the sweat smearing visibly across his forehead. He looks
straight ahead through the glass door toward the plunge room; his expression softens into
something close to affection — you and me again — a tiny private almost-smile flickers and
disappears. He leans forward, elbows on knees, and shakes his arms out loosely and gently,
a relaxed loosening-up with minimal movement, shoulders dropping, one long warm audible
exhale. He sits back up, looks at the door handle, and reaches for it slowly and casually
with one hand, the way you reach for a coffee mug; his hand wraps around the handle, he
pauses, one more small smile — here we go again — and the frame holds.

Camera law: locked-off tripod, 35mm prime, eye level, absolute rock-solid stillness from
first frame to last — zero drift, zero shake, zero stabilization float, zero pan, tilt,
zoom, dolly or breathing. The clip closes on precisely the framing it began with.

Warm-tungsten grade, hot amber palette, low-key and slightly underexposed so the heat
reads intense rather than bright; halation on the heater stones, haze softening the
background. Audio: diegetic ambient only — low sauna hum, dry heat hiss, distant water
circulation, his quiet breath, one long exhale at the arm shake. No music, no score, no bgm.

Count of men in frame: one. Count of glasses anywhere in frame: zero — his face stays
bare. Count of towels on his body or in his hands: zero. Count of rowing motions, arm
swings, or vigorous arm movements: zero — all movement stays slow, loose and casual.
Benches remain solid built-in furniture. Every expression reads as warm amusement at his
own theatrics, never grim, never heroic.
```

---

## What this prompt got right (the reusable lessons)

1. **Prose, not bullets.** The same locks written as a `CRITICAL LOCKS:` list scored 4.5/6. Written as sentences inside the description, 8.5/9.
2. **The absence sentence.** *"Nothing on his face, nothing draped over his shoulder, nothing in his hands."* One flat inventory line deleted the towel and glasses that the reference image and prior attempts kept reintroducing.
3. **Sweat stated four separate times**, in four different paragraphs, in four different phrasings. The single most-repeated requirement is the one that landed.
4. **The motion is disarmed by analogy, not by negation.** *"the way you reach for a coffee mug"* killed the rowing motion that *"NO rowing motion"* could not.
5. **Register embedded in the beat, not appended.** *"a tiny private almost-smile"* and *"you and me again"* carry the tone inside the action instead of instructing the model to feel something.
6. **Count locks last.** A short numeric coda after all the prose, so the final thing the model reads is the hard constraints.

## Only remaining soft miss

Visible steam wisps read as warm atmosphere rather than distinct curling steam. Acceptable
here. For S5B and S5D (steam room) the steam needs to be a described *physical obstacle* he
navigates, not an atmospheric adjective.


---

## Note on the reference swap (2026-09-03)

This prompt was originally sent with `Man-Swim-v2.png` — the younger recast man. **The
render came back as Seth anyway.** Frame-checked at 6s: receding hairline, thinning crown,
late-30s/early-40s face, short scruff. The model pulled the older read despite the younger
plate.

That is a useful data point and a warning in equal measure. The plate is the strongest
lever we have, but it is not absolute — a 12s video generation re-derives the face every
frame and can land somewhere between the plate and the prose. Here it landed on our side.
It won't always.

For any re-run of this shot, use `Seth-Swim-Bare.png`. The existing keeper stands as-is;
it already looks like him.
