# S3B — The Toe Dip and the Recoil (Scene 3, beat 2 of 4)

**Final duration in the cut:** ~3s, extracted from the 12s generation.
**Continues directly from S3A** — same room, same camera position, same standing spot.

**Attach from `refs/`, in this order:**

| Slot | File |
|---|---|
| Image 1 | `Seth-Swim-Glasses.png` |
| Image 2 | `Cold-Plunge-Room.png` |

**Settings:** `seedance_2_0` · `mode: std` · `genre: comedy` · `generate_audio: false`
· 12s · 1080p · 16:9

**The beat:** Seth lowers one foot until his toes break the surface, and his body
withdraws before he's decided to withdraw. Then he looks at his own foot as though it
acted without him.

**The failure this is written against.** The original Scene 3 recoil was rejected as
*"exaggerated and fake-looking — the model is doing surprised as a performance."* The
correction is that the recoil is **involuntary and small**: a knee bending, a foot lifting
an inch, over before it reads as a reaction. Nothing theatrical, no gasp, no full-body
flinch. The comedy is that his body has an opinion and he finds it mildly interesting.

**Water contact is intentional here** — unlike S3A, where zero contact was mandatory. But
it is toes only, for under a second, and he never gets past the ball of his foot.

---

## THE PROMPT

```
Seth lowers one bare foot toward the cold plunge, lets his toes touch the surface, and his
leg withdraws on its own before he has decided anything — then he looks down at his own
foot with mild interest, as if it had acted without consulting him.

The shot lives inside Image 2 exactly: an upscale indoor spa room in warm neutral tones.
An octagonal plunge pool sits in the near foreground, its interior lined with small blue
mosaic tiles, the water clear and still and pale cyan, the coping a band of dark polished
stone with no markings of any kind on it. Two curved brushed-stainless handrails rise out
of the pool. A neat stack of folded white towels sits on the deck at the left edge of the
pool, undisturbed. Further left, a large fiddle-leaf plant in a white cylindrical pot
stands beside a dark-framed glass sauna door, the cedar interior glowing warm amber behind
the glass. The right wall is floor-to-ceiling white marble with grey veining. In the middle
distance a second soaking pool sits against a dark stone wall, faint steam drifting off its
surface. The ceiling is beige tile with recessed round downlights; a linear LED strip runs
along the upper right. The floor is large-format beige stone tile, slightly damp and
reflective near the pool edge. Cool even daylight-balanced spa lighting, soft speculars on
the handrails and on the water, gentle reflections rippling on the ceiling.

Seth is Image 1 exactly: early forties, slender and untrained with narrow shoulders and a
soft midsection, dark brown hair short at the sides and tousled on top, clearly receding at
the temples, a short patchy reddish-brown stubble beard, matte organic skin with visible
pores, natural asymmetry and faint redness at the knees and elbows. He wears black
rectangular eyeglasses; the lenses are perfectly clear and completely unfogged — this room
is cold and nothing steams them. He is shirtless in plain navy-blue swim trunks, barefoot,
and his skin is dry. Nothing is draped over either shoulder, nothing is in his hands, no
towel touches his body at any point.

One continuous static shot, 0s to 12s — wide shot, full figure head to toe, eye level,
35mm, the frame identical at the end to the first pixel. The plunge pool occupies the lower
third of the frame; Seth stands frame-center on the near deck, already stopped, facing the
water, exactly where he came to rest a moment ago. He shifts his weight onto his left foot
and raises his right foot a few inches, holding it out over the water without hurry, the
sole angled down. He lowers it slowly. The moment his toes meet the surface the leg comes
back — a small involuntary withdrawal, the knee bending, the foot lifting perhaps four
inches and returning to the stone, the whole movement over in a fraction of a second. His
shoulders stay still. His face does not perform surprise; it barely changes. He looks down
at his own foot, then at the water, then at his foot again, with the mild interest of a man
noticing an unfamiliar reflex. His eyebrows lift a few millimetres. He shakes the foot once,
loosely, the way you shake off water. He plants both feet, looks at the water again, and a
small private almost-smile arrives at one corner of his mouth and does not become a grin.
He stays standing there, unbothered, and the frame holds.

Camera law: locked-off tripod, 35mm prime, eye level, absolute rock-solid stillness from
first frame to last — zero drift, zero shake, zero stabilization float, zero pan, tilt,
zoom, dolly or breathing. The clip closes on precisely the framing it began with.

Cool clean spa grade, neutral daylight white balance, gentle contrast, documentary realism
with fine natural grain; the cyan of the water is the only saturated colour in the frame.
Intended sound for post, not to be generated: quiet room tone, pool circulation hum, the
small slap of a toe breaking water, one short exhale.

Count of people in frame: one. Count of towels touching Seth's body or in his hands: zero.
Count of body parts in the water below the ball of his foot: zero — his toes touch the
surface and nothing more, no ankle, no calf, no knee, and he never steps in. Count of
readable letters, numbers, depth markers or signage anywhere in frame: zero. Count of
camera moves: zero. Count of fogged lenses: zero. Count of gasps, flinches, full-body
jolts, arm-flails, hops or theatrical recoils: zero — the withdrawal is a small reflex in
one leg and nothing else moves. Every expression reads as mild curiosity and private
amusement, never grim, never shocked, never played for the back row.
```

---

## Verification checklist

Frames at 2s, 4s, 5s, 7s, 10s.

| # | Check | Pass |
|---|---|---|
| 1 | Toes only — never past the ball of the foot, never steps in | ☐ |
| 2 | Zero readable text anywhere, background included | ☐ |
| 3 | Glasses present and clear, never fogged | ☐ |
| 4 | **Recoil is small and involuntary — no gasp, flinch, jolt or hop** | ☐ |
| 5 | Face matches the plate — receding hairline, patchy stubble, early forties | ☐ |
| 6 | Skin matte, not waxy | ☐ |
| 7 | No towel on his body | ☐ |
| 8 | Register curious/amused, never shocked or grim | ☐ |
| 9 | Camera dead static, first frame = last frame | ☐ |
| 10 | Audio track is silent or absent | ☐ |

**Pass threshold:** 8/10, with checks 1, 2, 3 and 4 mandatory. Check 4 is the whole point
of the shot — a theatrical recoil fails it regardless of the other scores.

**Save as:** `outputs/S3B-v1.mp4`

**Camera-lock note for whoever verifies:** measure SSIM on a static crop that contains no
water and no subject — the upper-left wall and plant area works. A whole-frame SSIM is
dragged down by water movement and reads as camera drift when the camera is locked.
