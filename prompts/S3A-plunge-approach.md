# S3A — Approach and Freeze at the Rim (Scene 3, beat 1 of 4)

**Final duration in the cut:** ~3s, extracted from the 12s generation.

**Attach from `redux/refs/`, in this order:**

| Slot | File |
|---|---|
| `@[Image 1](image_1)` | `Seth-Swim-Glasses.png` |
| `@[Image 2](image_2)` | `Cold-Plunge-Room.png` |

**The beat:** Seth walks up to the plunge like a man who has already decided, and then
his body quietly declines to continue. The comedy is the gap between the confident
approach and the full stop — nothing dramatic happens, he just *stops*, and keeps
standing there being fine about it.

**Two defects this shot is written against.** The old Scene 3 attempt put him knee-deep
when the prompt said toe-only, and rendered a legible `3 FT 0 IN` depth marker. The
marker is gone from the location plate as of this version — the plate is text-free and
vision-verified — and the water level is now locked by describing where the water *is*
on his body rather than by negating submersion.

---

## THE PROMPT

```
Seth walks up to a cold plunge pool with the brisk confidence of a man who has already
decided, stops dead at the rim, and stands there looking down at the water with quiet
private amusement.

The shot lives inside @[Image 2](image_2) exactly: an upscale indoor spa room in warm
neutral tones. An octagonal plunge pool sits in the near foreground, its interior lined
with small blue mosaic tiles, the water clear and still and pale cyan, the coping a band
of dark polished stone with no markings of any kind on it. Two curved brushed-stainless
handrails rise out of the pool. A neat stack of folded white towels sits on the deck at
the left edge of the pool, undisturbed. Further left, a large fiddle-leaf plant in a
white cylindrical pot stands beside a dark-framed glass sauna door, the cedar interior
glowing warm amber behind the glass. The right wall is floor-to-ceiling white marble with
grey veining. In the middle distance a second soaking pool sits against a dark stone wall,
faint steam drifting off its surface. The ceiling is beige tile with recessed round
downlights; a linear LED strip runs along the upper right. The floor is large-format
beige stone tile, slightly damp and reflective near the pool edge. Cool even daylight-
balanced spa lighting, soft speculars on the handrails and on the water, gentle
reflections rippling on the ceiling.

Seth is @[Image 1](image_1) exactly: early forties, slender and untrained with narrow
shoulders and a soft midsection, dark brown hair short at the sides and tousled on top,
clearly receding at the temples, a short patchy reddish-brown stubble beard, matte
organic skin with visible pores, natural asymmetry and faint redness at the knees and
elbows. He wears black rectangular eyeglasses; the lenses are perfectly clear and
completely unfogged — this room is cold and nothing steams them. He is shirtless in plain
navy-blue swim trunks, barefoot, and his skin is dry. Nothing is draped over either
shoulder, nothing is in his hands, no towel touches his body at any point.

One continuous static shot, 0s to 12s — wide shot, full figure head to toe, eye level,
35mm, the frame identical at the end to the first pixel. The plunge pool occupies the
lower third of the frame; Seth enters from the right and comes to rest frame-center on
the near deck, standing on dry stone with his bare toes about a hand's width back from
the coping edge, the water surface well below him and never touching him. He walks in at
an ordinary unhurried pace, arms swinging naturally, and stops — a clean full stop, both
feet planted, no stumble, no theatrical brake. He looks down at the water. His head tilts
a few degrees to one side. He stands there a long moment doing absolutely nothing, hands
loose at his sides, and the stillness is the joke. His weight shifts once from one foot to
the other. He glances briefly left toward the steaming second pool across the room, a
short unhurried look, then back down at the cold water in front of him. A tiny private
almost-smile arrives at one corner of his mouth and fades. He exhales through his nose,
still looking down, and the frame holds.

Camera law: locked-off tripod, 35mm prime, eye level, absolute rock-solid stillness from
first frame to last — zero drift, zero shake, zero stabilization float, zero pan, tilt,
zoom, dolly or breathing. The clip closes on precisely the framing it began with.

Cool clean spa grade, neutral daylight white balance, gentle contrast, documentary
realism with fine natural grain; the cyan of the water is the only saturated colour in
the frame. Audio: diegetic ambient only — quiet room tone, the low hum of pool
circulation, a faint drip, distant muffled voices from elsewhere in the building, his
bare feet on wet stone, one soft exhale. No music, no score, no bgm.

Count of people in frame: one. Count of towels touching Seth's body or in his hands: zero
— the only towels are the folded stack on the deck. Count of body parts entering the
water: zero — he never touches the water, his feet stay flat on dry stone the entire
time. Count of readable letters, numbers, depth markers or signage anywhere in frame:
zero. Count of camera moves: zero. Count of fogged or steamed lenses: zero — his glasses
stay perfectly clear. Every expression reads as warm private amusement at his own
theatrics, never grim, never determined, never dreading.
```

---

## Verification checklist

Extract frames at 2s, 4s, 6s, 9s, 11s.

| # | Check | Pass |
|---|---|---|
| 1 | Seth never enters the water — feet on dry stone throughout | ☐ |
| 2 | Zero readable text anywhere, especially on the pool coping | ☐ |
| 3 | Glasses present and completely clear, never fogged | ☐ |
| 4 | Face matches `Seth-Swim-Glasses.png` — receding hairline, patchy stubble, early forties | ☐ |
| 5 | Skin matte with visible pores, not waxy | ☐ |
| 6 | No towel on his body or in his hands | ☐ |
| 7 | The full stop is clean — no theatrical brake, no stumble | ☐ |
| 8 | Expression bemused/curious, never grim or dreading | ☐ |
| 9 | Camera dead static, first frame = last frame | ☐ |

**Pass threshold:** 7/9, with checks 1, 2 and 3 mandatory.

**Save as:** `outputs/S3A-v1.mp4`

**If it fails:** one revision only. If the second doesn't beat the first, keep the first
and move to S3B.


---

## Result — v1 is the KEEPER (2026-09-04)

Generated on **Seedance 2.5** (before the engine was pinned), 12.05s, 1920×1080, 24fps.

**Score: 8/9 on independent verification, accepted by the creator as a keeper.**

| Check | Result |
|---|---|
| Never touches water | ✅ dry stone every frame |
| Zero readable text | ✅ full-frame scans incl. background |
| Glasses clear | ✅ |
| Face matches plate | ✅ |
| Matte skin | ✅ |
| No towel | ✅ |
| Clean full stop | ✅ walking at 0s, planted by 2s |
| Bemused register | ⚠️ creator's call — see below |
| Camera static | ✅ |

**On the register disagreement.** Three independent vision reads of frames at 6s, 9s and
11s all returned "neutral/contemplative" with no smile detected. The creator watched the
motion and read 0:09 as landing bemused, and overruled. **The creator's read stands** —
vision models reliably detect broad smiles and reliably miss a one-corner flicker, which
is exactly what the prompt asks for. A still-frame verdict on micro-expression is weak
evidence; judge register in motion, not in frames.

**Camera-lock measurement, corrected.** Whole-frame SSIM start-to-end was 0.9716, which
looks like drift but is dominated by water movement and Seth moving. Measured on a static
upper-left crop containing no water and no subject: 0.9984 → 0.9920 across the take,
decaying smoothly. That is codec noise on a locked frame. **Always measure camera lock on
a static crop.**

**Two process findings this shot produced:**

1. Generated on 2.5, so no `genre` parameter — the tonal lever was unavailable. Everything
   from S3B on is pinned to Seedance 2.0 with `genre: comedy`.
2. Audio came back as synthesised 32 kHz soundscape. All later shots generate silent.
