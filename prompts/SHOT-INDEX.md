# Redux shot index — 108-second film, rebuilt shot by shot

**Method:** every shot is one locked-off 12s generation in the seven-paragraph shape
(`../PROMPT-SHAPE.md`), sent one at a time to a Higgsfield Super Computer session primed
with `00-SUPERCOMPUTER-INTRO.md`. Multi-beat scenes split into sub-shots, cut in POST.
Nothing generated from a previous attempt's context.

**Character:** Seth — see `../SETH.md`. All six wardrobe plates derive from one face.

**Naming:** `S<scene><letter>`. Prompts at `prompts/<shot>-<slug>.md`, outputs at
`outputs/S3B-v1.mp4`.

---

## Phase 1 — The setup (Scenes 1–2)

| Shot | Beat | Seth plate | Location | Glasses | Status |
|---|---|---|---|---|---|
| **S1** | Car: the lie, and the look-up | `Seth-Car.png` | `Lifetime-Fitness-Exterior.jpeg` | on | prompt ready |
| S2A | Court portrait, two bounces, serve into the net tape | `Seth-Gym.png` | `Pickleball-Courts.png` | on | queued |
| S2B | The two ladies: sharp exhale, flat appraising stare | `Senior-Lady-Lavender/Plum.png` | `Pickleball-Courts.png` | — | queued |
| S2C | The whiff, then the stiff respectful nod | `Seth-Gym.png` | `Pickleball-Courts.png` | on | queued |

## Phase 2 — The water and heat block (Scenes 3–6)

| Shot | Beat | Seth plate | Location | Glasses | Status |
|---|---|---|---|---|---|
| S3A | Confident approach, freeze at the rim | `Seth-Swim-Glasses.png` | `Cold-Plunge-Room.png` | clear | ✅ **KEEPER v1** 2026-09-04 |
| **S3B** | Bare toe dip, behavioural recoil | `Seth-Swim-Glasses.png` | `Cold-Plunge-Room.png` | clear | **next** |
| S3C | Pacing, murmured pep talk, the glance at the hot tub | `Seth-Swim-Glasses.png` | `Cold-Plunge-Room.png` | clear | queued |
| S3D | Grips the rail, foot hovers and locks | `Seth-Swim-Glasses.png` | `Cold-Plunge-Room.png` | clear | queued |
| **S4** | Sauna psych-up — **LOCKED KEEPER, 8.5/9** | `Seth-Swim-Bare.png` | `Sauna-Interior.png` | off | locked |
| S5A | Temptation at the plunge rim | `Seth-Swim-Glasses.png` | `Cold-Plunge-Room.png` | clear | queued |
| S5B | Steam room navigation — **lenses white out** | `Seth-Swim-Glasses.png` | `Steam-Room.png` | fogging | queued |
| S5C | Sauna lounging, elbows on knees | `Seth-Swim-Glasses.png` | `Sauna-Interior.png` | fogged | queued |
| S5D | Steam room, the slow resigned lens wipe | `Seth-Swim-Glasses.png` | `Steam-Room.png` | wipe → refog | queued |
| S5E | Rear shot: feet in the plunge, staring at the hot tub | `Seth-Swim-Glasses.png` | `Cold-Plunge-Room.png` | n/a (rear) | queued |
| S6A | Foot in for real, the grimace, the U-turn | `Seth-Swim-Glasses.png` | `Cold-Plunge-Room.png` | clear | queued |
| S6B | Hot-tub collapse, steam rising | `Seth-Swim-Glasses.png` | `Cold-Plunge-Room.png` | fogging | queued |

## Phase 3 — The comedown (Scenes 7–9)

| Shot | Beat | Seth plate | Location | Glasses | Status |
|---|---|---|---|---|---|
| S7A | The forensic bottle investigation | `Seth-Shower.png` | `Shower-Room-Closed-Door.png` + `Bottles-Blank-Label.png` | **off, on the ledge** | queued |
| S7B | Three confused pumps, bewilderment at the volume | `Seth-Shower.png` | same | off | queued |
| S8A | Serene stroll into an aisle of identical lockers | `Seth-Towel.png` | `Locker-Room.png` | on | queued |
| S8B | The combination lock: spin, tug, nothing | `Seth-Towel.png` | `Locker-Room.png` | on | queued |
| S8C | Puffed-cheek exhale, reset to zero, slower | `Seth-Towel.png` | `Locker-Room.png` | on | queued |
| **S9** | The bar, from behind: content, then the reply | `Seth-Car.png` | `Bar-Area.png` | on | queued |

**24 shots. 22 to generate** (S4 locked, S1 written). Floor ~2,400 credits, ceiling ~4,750
at the two-attempt rule. Balance after the cast rebuild: **9,384**.

---

## Generation settings (every shot)

`seedance_2_0` · `mode: std` · `genre: comedy` · `generate_audio: false` · 12s · 1080p · 16:9

**`genre: comedy` is proven here, with one open risk.** Both Scene 7 generations that used
it passed their register check as genuinely bemused — no broad playing, no slapstick. S3A,
generated on Seedance 2.5 without it, came back tonally flat. Treat it as a grade and
pacing hint, not a performance instruction; the slapstick risk lives in prompt language
("stumbles", "comically", "flails"), which our prompts never use.

**Open risk — watch S2A/S2C and S6A.** The evidence covers static, contemplative shots
only. The two shots with real physical action (the pickleball whiff; the foot hitting cold
water and the body jolting) are where a model could decide "comedy" means broad. If either
comes back mugging, drop that shot to `genre: auto` — one parameter, no prompt rewrite.

**Always generate silent.** S3A's synthesised audio was 32 kHz machine-generated
soundscape. The Scene 7 canary that passed 6/6 used `generate_audio: false`. All sound is
Phase 4 post; the audio paragraph in each prompt is a note for the editor, not a
generation instruction.

## The glasses arc (track it across shots)

Clear in the cold plunge → white out in the steam → wiped and refogged → off for the
sauna and shower → back on for the locker room. S7 is the payoff: they're on the ledge,
he can't read the bottles, he pumps all three. Do not let a shot fog them unasked.

## POST assembly (after generation, not before)

Scenes 1, 4 and 9 run full-length; 2, 3, 5, 6, 7, 8 concatenate from sub-shots. Text
overlays, typing animation and sound sync are Phase 4 and start only when every shot is
a keeper.

## Rules carried forward

- Two attempts maximum per shot. If the second doesn't beat the first, keep the first.
- Never spend a second video attempt against a reference defect. Fix the plate (2–9 credits), then one video (108).
- Never generate readable text anywhere.
- Every expression lives in the bemused band. Grim is a failed generation even if everything else passes.
- **NSFW classifier:** don't *generate* shirtless full-body plates — GPT Image 2 refuses. Edit an approved plate with Nano Banana Pro instead.
- **Scrub text from location plates before shooting them.** `Cold-Plunge-Room` had legible `3 FT 0 IN` / `3 FT 8 IN` / `NO DIVING` markings and the old Scene 3 render reproduced them. Text in a plate is inherited exactly like waxy skin is. Scrubbed version installed 2026-09-03; original in `_retired/`.
