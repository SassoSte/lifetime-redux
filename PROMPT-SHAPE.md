# The redux prompt shape (binding)

Derived from the prompt that produced the Scene 4 keeper (8.5/9,
`hf-man-in-sauna.mp4` = `scene-4-attempt-3-external-2026-09-03.mp4`, md5 verified
identical). Every redux shot prompt is written in exactly this shape — seven
paragraphs, flowing prose, no bullet lists, no timecode tables.

Prose beats what bulleted specs. The bulleted `CRITICAL LOCKS:` / `[0s–3s]` format
from the 2026-09-03 prompt set scored 4.5/6; the same content written as continuous
sentences scored 8.5/9. Keep it prose.

---

## Paragraph 1 — Logline

One sentence. Subject, register, location, the three or four physical events, in order.
Always opens with the tonal word: *"A bemused man…"*

> A bemused man steels himself in a hot sauna for the cold plunge waiting beyond the
> glass door — breath work, streaming sweat, a small private smile, and one slow reach
> for the handle.

## Paragraph 2 — The set

Opens `The shot lives inside @[Image 2](image_2) exactly:` then the room in one long
sentence of concrete nouns — materials, geometry, where things sit relative to frame.
Then light. Then atmosphere (haze, shimmer, steam, spill). Then the undisturbed props
that prove the room is lived-in.

## Paragraph 3 — Seth

Opens `Seth is @[Image 1](image_1) exactly:` then age, build, hair, stubble, skin
texture, eyes. Then the **absence sentence** — a flat inventory of what is *not* there:
*"Nothing draped over his shoulder, nothing in his hands."* Then wardrobe. Then his
physical condition in this shot (wet with sweat / dry / damp hair / dressed), and the
state of his glasses (clear, fogged, absent, in hand).

The absence sentence is load-bearing. Reference plates and the model's own priors keep
reintroducing towels; the prompt has to actively delete them.

**Name him.** Use "Seth" throughout the beats rather than "the man." A named character
gets more consistent performance out of the model than a described one — the name acts
as a single handle for face, build and register instead of three separate constraints
the model re-derives each sentence.

## Paragraph 4 — The take

Opens `One continuous static shot, 0s to 12s —` then framing, lens height, staging
(where he sits/stands, what is background-left, background-right). Then the beats as
continuous prose, each linked by a verb, each carrying its own micro-expression. No
timecodes. End on the frame holding.

Aim for four to six beats. One motion. If it needs a cut, it is two shots.

## Paragraph 5 — Camera law

Verbatim, every time:

> Camera law: locked-off tripod, 35mm prime, eye level, absolute rock-solid stillness
> from first frame to last — zero drift, zero shake, zero stabilization float, zero pan,
> tilt, zoom, dolly or breathing. The clip closes on precisely the framing it began with.

Vary only lens and height when a shot genuinely needs it, and say why in the notes.

## Paragraph 6 — Grade and audio

Grade, palette, exposure intent, one optical note (halation, haze, roll-off). Then
`Audio: diegetic ambient only —` a short list. Always close with
`No music, no score, no bgm.`

## Paragraph 7 — Count locks

Literal counts, semicolon-separated, each `Count of X in frame: N`. Include at minimum
people, glasses, towels, and whatever failure mode this specific shot is prone to
(rowing motions, submersion, readable text, camera moves). Close with the register
sentence: *"Every expression reads as warm amusement at his own theatrics, never grim,
never heroic."*

---

## Reference convention

| Slot | Always |
|---|---|
| `@[Image 1](image_1)` | Character |
| `@[Image 2](image_2)` | Location |
| `@[Image 3](image_3)`+ | Props / second character |

Attach from `redux/refs/` only. Max 9 per job. Do not attach a hero sheet and a
wardrobe variant in the same job — they fight.

## Anti-patterns (each one cost a generation)

- Bulleted `CRITICAL LOCKS` blocks — the model skims them. Fold the lock into the prose sentence that describes the thing.
- Timecode tables — they invite the model to cut.
- Negations without a positive replacement. "No towel" alone leaves a towel-shaped hole; "nothing draped over his shoulder, his shoulders bare and wet" fills it.
- Describing a fix for a reference-image defect. Waxy skin, garbled labels and open doors are inherited from the reference and are not prompt-fixable. Fix the image.
- More than one location, or more than one camera setup, in one generation.

<!-- publish-test -->
