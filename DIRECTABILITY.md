# The Directability Ceiling

**Written 2026-09-04, at the point of pausing this film.** Read this before attempting
another shot. It is the most expensive thing learned here and it is not in any prompting
guide.

## The finding

**Current text-to-video models render *states* reliably and *events* unreliably.**

You can specify a situation — a man, a sauna, warm amber light, a locked camera, a bemused
register held for twelve seconds — and get a beautiful rendering of it. You cannot reliably
specify a performance: this action, at this moment, at this speed, with this expression
arriving a beat after that one.

The model has its own centre of gravity. Prompt language perturbs it. It does not relocate
it.

## The evidence

Same prompt discipline, same day, same project, same operator:

| Shot | Ask type | Result |
|---|---|---|
| S4 sauna | **state** — sitting, sweating, steeling himself | 8.5/9 keeper |
| S7 shower | **state** — regarding bottles with quiet focus | 6/6, twice |
| S3A plunge approach | **state** — walks in, stops, stands there | 8/9 keeper |
| S3B toe dip | **event** — contact and recoil, sub-second | 3 attempts, 3 failures |

The toe dip is not exotic. A man touches cold water and flinches.

| Attempt | Asked | Rendered |
|---|---|---|
| Scene 3, Sep 3 | toe dip, feet/ankles only | knee-deep submersion |
| S3B v1 | fast involuntary recoil | slow exploratory hover, toes held above the surface — "like an alien creep" |
| S3B v2 | explicit zero-hover count, fast binary contact | **two** mid-air holds (5 frames at 4.12–4.33s, 9 frames at 4.54–4.92s), then a step-in with a bracing crouch |

Every escalation available was applied: prose instead of bullets, the action moved to the
first paragraph and made the majority of the sentences, numeric zero-counts (*"Count of
seconds his foot spends hovering above the water without touching it: zero"*), analogy
instead of negation, physical staging instead of prohibition, and a new intro section on
physical honesty.

The model rendered **"man slowly entering a pool"** all three times, because that is the
dominant prior for `man + cold plunge + foot`.

## Why the state/event line is the real boundary

The shots that worked ask for a **condition**. Sitting in a sauna sweating. Standing at a
rim looking down. Regarding three bottles with quiet focus. Conditions render beautifully —
the model holds a mood for twelve seconds very well.

The shot that failed asks for an **event with internal timing**: a toe touches water and
withdraws in under half a second, a wince at the instant of contact, amusement a beat
later. Three things in sequence, each with a duration.

That is where directability collapses. Not because the shot is hard to imagine, but because
timing is not an exposed parameter — it is text to be interpreted, and interpretation is
where the prior wins.

## The corollary about published AI video

The extraordinary AI video circulating publicly is largely **not directed**. The engine
proposes, the human selects, and the edit is assembled from what came back. Volume plus
curation, not specification.

That is a legitimate and powerful workflow. It is simply not the same craft as directing.
Conflating them is what makes the tooling feel broken when you arrive with a storyboard.

**If you have a shot in your head, you are working against the grain. If you are willing to
discover the shot in what returns, you are working with it.**

## Practical rules that follow

**Write for states, not events.** If a beat is "this, then that, a beat apart," it is at
high risk. Prefer beats the model can *hold* over beats it must *execute*.

**Budget by prior strength, not perceived difficulty.** "Man sweating in a sauna" is cheap
because the prior is aligned. "Toe touches water and snaps back" is expensive because the
prior fights it. How hard the shot looks to *you* is not the cost driver.

**Two attempts, and mean it.** Three attempts at the toe dip produced three variations of
one failure. The third was not closer than the first. When two attempts fail *the same
way*, the prior is the problem and a third attempt is just money.

**Fix plates, not prompts.** Waxy skin, garbled labels and baked-in text are all
reference-inherited. 2–9 credits on the image beats 108 on the prompt, every time.

**Plates are not absolute either.** The S4 keeper was generated with the wrong (younger)
character plate and rendered the older man anyway, because the prose described him. A 12s
generation re-derives the subject every frame and lands between plate and text.

**Cutting a beat is a legitimate creative response.** Scene 3 needed ~3s from the toe dip.
S3A's dead stop and the following shot's pacing can carry the same hesitation. An
undirectable beat is information about the beat, not only about the tool.

## When to revisit

The gate is not better prompting. It is **models that expose timing and performance as
controllable parameters** — keyframe-level direction, per-beat timing, expression curves —
rather than as prose to be interpreted. Watch for that capability by name. Higher fidelity,
longer clips and better resolution do not address it.

Until then the honest options are: work in states, curate volume, or wait.

## Vault

Full version, with the verification discipline and model-selection facts:
`07 Reference/AI Video — The Directability Ceiling.md` in the Obsidian vault.
