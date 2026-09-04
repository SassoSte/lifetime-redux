# Seth — the working character sheet

**This file replaces `character-bible.md` for the redux track.** The old bible describes a
different man (bald, pale-blue eyes, thin amber Danish frames) — that was the locked
casting for the retired shot-by-shot track and it never matched the 108-second film. Do
not reconcile them. This is the man who is actually on screen.

---

## Who he is

**Seth.** Early forties. The responsible novice everyman. He joins because exercising is
the right thing to do, arrives with a reasonable plan, and has no idea the club requires
its own advanced form of time management. The place happens *to* him.

He is not bad at ordinary life. Each delay is rational in isolation — try the cold plunge,
stay a few more minutes in the steam, work out which bottle is which. The accumulation
creates the time warp. Negligence or stupidity breaks the role; the comedy is always on
the club, never on him.

**The register, which matters more than any physical detail:** he is not suffering, he is
enjoying his own bewilderment. Warm amusement at his own theatrics. "Here we go again."
Never grim, never heroic, never condemned, never satisfied.

## What he looks like

Dark brown hair, short at the sides, a little tousled on top, clearly receding at the
temples and thinning at the crown. High lined forehead. Short patchy reddish-brown
stubble beard, a few greys at the chin. Moderately thick dark eyebrows, straight nose,
squarish jaw softened by age, ears that protrude slightly. Black rectangular eyeglasses.

Build of a man who does not train: slender arms, narrow chest, soft midsection with an
ordinary small belly, no abdominal definition, faint slouch.

**Four permanent negatives:** never younger, never a full head of hair, never
clean-shaven, never muscle definition. These are the four directions the model drifts.

## Wardrobe plates — `refs/` is the authority

| Plate | Scenes | Glasses |
|---|---|---|
| `Seth-Car.png` | S1, S9 | on |
| `Seth-Gym.png` | S2 | on |
| `Seth-Swim-Glasses.png` | S3, S5, S6 | on, clear |
| `Seth-Swim-Bare.png` | S4 | off |
| `Seth-Shower.png` | S7 | off |
| `Seth-Towel.png` | S8 | on |

All six derive from the same face. The plate wins over any prose description, including
this file. Prose exists to stop drift, not to define him.

## The glasses

His only real prop, and the one running gag the physical design supports. He wears them
everywhere except in water and in the shower.

- **Cold plunge (S3):** clear. Cold room, no fog. This is the baseline the steam plays against.
- **Steam room (S5B, S5D):** they white out on entry. He navigates blind, wipes them on the back of his hand, they fog again in about two seconds. He keeps going.
- **Sauna (S4):** off. He's come from the water.
- **Shower (S7):** off, and sitting on the ledge just out of reach. He cannot read the bottles. That is the whole joke — he doesn't *choose* three products, he can't tell them apart.
- **Locker room (S8):** back on, and the combination lock still defeats him.

**Physical accuracy note for prompts:** real lenses fog on the *inside*, from *below*,
clouding upward, and clear from the outer edges inward. Models default to a uniform white
haze over the whole lens, which reads as a filter rather than as steam. Specify it.

---

## Why the old bible failed, honestly

The old bible specified a bald man with pale-ice-blue eyes and thin amber Danish frames,
reasoning that a low-drift-surface face would generate consistently. The film's man has
hair, a receding hairline and black frames. The spec never survived contact with the
generator.

The correction is not a better-written bible. **Consistency comes from reference plates,
not from prose.** A described character is re-derived on every generation and drifts every
time; a plate is a fixed input. The Sep 2 hero-sheet rebuild proved this in the other
direction — it fixed waxy skin and silently recast him a decade younger, and nothing in
the bible stopped it, because nothing in the bible was an *input* to anything.

So this file is deliberately short. It carries the register, the four permanent negatives,
and the glasses device — the things a plate cannot encode. Everything visual lives in
`refs/`. When they disagree, the plate wins.

**Corollary worth remembering:** the model does enforce its own rules absolutely — the
NSFW classifier blocked two shirtless plates outright, no negotiation. It enforces safety
policy strictly and creative specification loosely. Design around that asymmetry rather
than against it.
