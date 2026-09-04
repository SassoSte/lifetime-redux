# S3B — The Toe Dip and the Recoil (Scene 3, beat 2 of 4) — v2

**Final duration in the cut:** ~3s, extracted from the 12s generation.
**Continues directly from S3A** — same room, same camera position, same standing spot.

**Attach from `refs/`, in this order:**

| Slot | File |
|---|---|
| Image 1 | `Seth-Swim-Glasses.png` |
| Image 2 | `Cold-Plunge-Room.png` |

**Settings:** `seedance_2_0` · `mode: std` · `genre: comedy` · `generate_audio: false`
· 12s · 1080p · 16:9

---

## Why v1 failed, and what changed

v1 rendered the foot **extended and hovering over the water, feeling for it, lingering** —
the creator's words: *"weirdly touching the water like he's an alien creep."* Motion
analysis across all 289 frames confirmed it: no discrete event anywhere, a flat curve. The
movement was slow and continuous, which is exactly the problem. Nobody explores cold water
with a hovering toe. You touch it and you are gone.

Two changes, and they are the whole rewrite:

**1. The contact is fast and binary.** Foot goes down, toe hits, foot is already coming
back. No hovering, no reaching, no feeling for the surface, no holding. The withdrawal is
faster than the approach.

**2. The cold is real, and the amusement is retrospective.** v1's prompt asked for mild
curiosity *at the moment of contact*, which produced a man serenely unbothered by ice
water — inhuman. The creator's correction: *"the look on a man's face when he experiences a
cold plunge is not bemusement at the moment his toe hits, but after, when he realizes it's
way harder than it looks."*

So the beat is now three-part: **honest flinch → recognition → private amusement.** The
wince is real and unperformed. The smile arrives about a second later, and it is a smile
at himself for having underestimated it.

There is precedent — `EDIT-NOTES` marked Scene 6's grimace *"good, real, keeper."* An
honest physical reaction is already approved for this film. The tonal law governs how Seth
*regards* things, not how his nervous system responds to them.

---

## THE PROMPT

```
Seth touches the cold plunge with one toe, snaps his foot back instantly with a real wince
at how cold it is, and then a second later starts quietly laughing at himself for having
thought it would be easy.

The action, in order, and it is the entire shot: he lifts one foot, lowers it directly to
the water, the toe breaks the surface, and the foot leaves immediately — the retreat is
faster than the approach and happens the instant contact is made. His face flinches
honestly at the cold, a sharp involuntary wince, eyes tightening, a hiss of breath through
his teeth. He plants the foot back on the stone. He looks at the water. And then it lands
on him — a small disbelieving shake of the head and a private almost-laugh, the expression
of a man who has just discovered that this is much harder than it looks.

Seth is Image 1 exactly: early forties, slender and untrained with narrow shoulders and a
soft midsection, dark brown hair short at the sides and tousled on top, clearly receding at
the temples, a short patchy reddish-brown stubble beard, matte organic skin with visible
pores and natural asymmetry. He wears black rectangular eyeglasses; the lenses are
perfectly clear and completely unfogged. He is shirtless in plain navy-blue swim trunks,
barefoot, skin dry. Nothing draped over either shoulder, nothing in his hands, no towel
touching his body at any point.

The shot lives inside Image 2 exactly: an upscale indoor spa room in warm neutral tones. An
octagonal plunge pool sits in the near foreground, interior lined with small blue mosaic
tiles, the water clear and pale cyan, the coping a band of dark polished stone with no
markings of any kind on it. Two curved brushed-stainless handrails rise out of the pool. A
neat stack of folded white towels sits on the deck at the left edge, undisturbed. Further
left, a large fiddle-leaf plant in a white cylindrical pot stands beside a dark-framed
glass sauna door, cedar interior glowing amber behind the glass. The right wall is
floor-to-ceiling white marble with grey veining. In the middle distance a second soaking
pool sits against a dark stone wall, faint steam drifting off it. Beige tile ceiling with
recessed round downlights, a linear LED strip upper right, large-format beige stone floor
tile slightly damp near the pool edge. Cool even daylight-balanced spa lighting, soft
speculars on the handrails and water.

One continuous static shot, 0s to 12s — wide shot, full figure head to toe, eye level,
35mm, the frame identical at the end to the first pixel. Seth stands frame-center on the
near deck, already stopped, facing the water, both feet flat on dry stone. He stands still
for a moment. Then he shifts his weight, raises his right foot, and takes it straight down
to the water without pausing and without hovering — no exploratory reaching, no feeling
for the surface, no holding it above the water. The toe touches. The foot is instantly gone,
snapping back up and onto the stone in a single fast reflex, quicker than it went down. At
the moment of contact his whole face reacts honestly: a hard involuntary wince, eyes
squeezing, teeth showing briefly, a sharp inward hiss of breath, shoulders jumping up
towards his ears once and dropping. It is genuine and it is not performed for anyone. He
stands there a beat with both feet planted, blinking, breathing out. He looks down at the
water again with something like respect. Then the recognition arrives and his face changes:
a slow disbelieving shake of the head, a huff of breath that is almost a laugh, and a small
private grin at his own expense — the look of a man who has just learned something about
himself. He is still grinning faintly, looking at the water, when the frame holds.

Camera law: locked-off tripod, 35mm prime, eye level, absolute rock-solid stillness from
first frame to last — zero drift, zero shake, zero stabilization float, zero pan, tilt,
zoom, dolly or breathing. The clip closes on precisely the framing it began with.

Cool clean spa grade, neutral daylight white balance, gentle contrast, documentary realism
with fine natural grain; the cyan of the water is the only saturated colour in the frame.
Intended sound for post, not to be generated: room tone, pool hum, the small slap of a toe
breaking water, a sharp inhale, a breathy laugh.

Count of people in frame: one. Count of towels touching Seth's body or in his hands: zero.
Count of body parts entering the water past the toes: zero — the toe touches the surface
and nothing more, no ball of the foot, no ankle, no calf, and he never steps in. Count of
seconds his foot spends hovering above the water without touching it: zero — the foot goes
straight down and comes straight back, no exploratory hover, no lingering, no feeling for
the surface, no holding. Count of readable letters, numbers, depth markers or signage
anywhere in frame: zero. Count of camera moves: zero. Count of fogged lenses: zero. Count
of smiles or amusement during the moment of contact: zero — the wince is honest, the
amusement comes afterwards. Count of full-body jolts, arm-flails, hops, backward stumbles
or comic double-takes: zero — the reflex is one sharp foot-and-shoulder reaction and
nothing more, and the laugh that follows is quiet and inward.
```

---

## Verification checklist

**Do not sample at fixed intervals for check 4 or 5.** The contact is under half a second.
Extract every 2nd frame from 3s to 9s and locate the motion spike first, then judge the
frames on either side of it.

| # | Check | Pass |
|---|---|---|
| 1 | Toe touches the water — the contact actually happens | ☐ |
| 2 | **No hovering.** Foot goes straight down and straight back; never holds above the surface | ☐ |
| 3 | Withdrawal is fast — retreat quicker than approach, one sharp reflex | ☐ |
| 4 | **Honest wince at the moment of contact** — not serene, not amused, not unbothered | ☐ |
| 5 | **Amusement arrives AFTER, ~1s later** — head shake, huff, private grin | ☐ |
| 6 | Never past the toes into the water; never steps in | ☐ |
| 7 | Zero readable text anywhere, background included | ☐ |
| 8 | Glasses present and clear | ☐ |
| 9 | Face matches plate; skin matte; no towel | ☐ |
| 10 | Camera dead static (measure on a static crop, not whole frame) | ☐ |
| 11 | No audio stream | ☐ |

**Mandatory: 2, 3, 4, 5.** Those four are the entire rewrite. A serene or lingering foot
fails the shot regardless of everything else.

**Verification method note:** ask *"describe what his foot and face do, second by second"* —
an open question. Do **not** ask *"is the recoil small and involuntary or theatrical?"*;
that is a forced choice between two answers, and a model handed the prompt's own vocabulary
will return it whether or not the action occurred. v1 was scored 10/10 that way and the
action was wrong.

**Save as:** `outputs/S3B-v2.mp4`
