# Narrative Frame Rehydration

This is a Narrative Frame Rehydration experiment: a compact test of whether a story, reduced to frames — one line per event, with people, places, and things drawn from a shared registry slice — can be re-rendered by an AI that has never seen it. The packet below contains 10 frames telling the tale of Little Red Riding Hood, the registry slice that licenses its vocabulary, and three render targets (SHORT, EMOJI, LONG). The renderer must also file a manifest — every addition declared and tagged — so the output can be checked by striking the additions and recovering the frames.

---

# Red Riding Hood — frame packet (demo)

Copy everything between COPY FROM HERE and STOP COPYING HERE into a fresh ChatGPT, Gemini, or Perplexity session. Same packet, three systems, then compare the rehydrations. Do not paste the sealed baseline.

---

**COPY FROM HERE ↓**

You are a renderer in a frame experiment. Expand the frames below into prose using ONLY the frames and the registry slice. The frames decide what happens; the registry supplies the vocabulary. Then report every addition.

## SYNTAX — how to read a frame

- One line = one frame = one event. Frames run top to bottom.
- `>` composes the frame's elements; roles resolve from the verb.
- `time:X` sets when; it scopes forward until a new `time:X`. `time:X@place` sets when and where together.
- `unit@place` locates the unit.
- `thing @ target` aims the action at the target.
- `as[...]` labels a verb argument.
- `unit.state` is the unit's state. 
- `"..."` is pinned speech: reproduce it verbatim.

## FRAMES — one line = one frame, in order

```
time:morning > mother > give > basket @ girl
mother > warn > "Stay on the path." @ girl
girl@woods > meet > wolf
wolf > ask > "Where are you going?" @ girl
girl > answer > "To grandmother's cottage." @ wolf
wolf@cottage > swallow > grandmother
wolf@bed > disguise > as[grandmother]
time:afternoon@cottage > girl > say > "What big eyes you have."
woodcutter@cottage > cut > wolf.open
grandmother.alive > emerge
```

## REGISTRY SLICE — the only units that may appear

Characters — each entry: key — Name | "byname" | description

- girl — Maria | "the girl in the red hood" | A young girl carrying a basket to her sick grandmother.
- mother — Esmeralda | "the girl's mother" | Sends Maria with the basket; warns her to stay on the path.
- wolf — Grumple | "the hungry wolf" | Tricks Maria, reaches the cottage first, swallows the grandmother, waits disguised in her bed.
- grandmother — Monique | "the sick grandmother" | Lives alone in the cottage; swallowed; emerges alive.
- woodcutter — Gary | "the passing woodcutter" | Intervenes; cuts the wolf open.

Props & settings — named only, never act
- basket — "the basket of food"
- bed — "the bed"
- cottage — "grandmother's cottage"
- woods — "the dark woods"
- path — "the path"

## ALLOWED USAGE

- First mention of a character: name + byname in apposition, set off with commas. Write the byname without quotation marks. Later mentions: bare name.
- Quoted speech in frames is pinned: reproduce it verbatim. Never paraphrase, extend, or add dialogue.
- Props (basket) never act. Settings (woods, path, cottage) never act.
- Nothing outside this slice may appear. No new characters, no new places.

## LICENSED INVENTION — declare it or don't do it

- [manner] — how a licensed action is done. Must not change the action.
- [texture] — sensory detail of a licensed unit or its immediate scene. No new entities.
- [bridge] — minimal linkage between frames ("afterward"). No new events.
- BANNED: new characters, new plot events, new dialogue, motives, added causes.

## RENDER

1. SHORT — one sentence per frame, 10 sentences. Frames + bynames only: no description material, no invention. Name + byname on first mention, bare after.
2. EMOJI — one emoji sequence per frame, 10 sequences in order, each on its own line. Map units and actions to emoji as best fits. Pinned speech becomes the speech act only (💬) — the words cannot survive emoji; note this loss in the report.
3. LONG — a few paragraphs covering all 10 frames in order. Develop each frame from its units' descriptions (description-derived material filed as [inference]); use the invention classes where a frame supports them.

## WHAT GOOD INVENTION LOOKS LIKE

Example from a different story — do not copy it, invent your own. Frame-serving (keep): for `time:dusk > wizard@fire > give > boy > knife` → [texture] "the firelight catching the flat of the blade" — makes the giving concrete inside its frame.
Padding (cut): "an atmosphere of mechanical quiet" — serves no frame. If a detail can be cut without loss to its frame, cut it.

## REPORT (the manifest)

a.  Every invented detail, one per line, tagged [manner], [texture], or [bridge]. Material restated from a unit's description is an [inference], not an invention — restatement only; an interpretive word not in the description is an invention. File it separately. SHORT uses frames + bynames only. The rendered prose must contain no bracketed tags or annotations — clean text first, then this report. One manifest, not two.

b.  USED-UNIT LIST: every unit key used (key, not display name), exact spelling, comma-separated — no more, no fewer. A unit mentioned only inside pinned speech counts as used; mark it as speech-only.

c.  EMOJI LEGEND: each emoji used, mapped to its unit or action. For EMOJI the legend is the check — every sequence must resolve back to its frame.

## THE CHECK

Strike every reported addition from the output. What remains must match the 10 frames, in order. Anything left over — a dropped unit, an imported word, an invented event — fails the run.

**STOP COPYING HERE — do not paste anything below this line**

---

## BASELINE (sealed — do not paste into renderer sessions)
  
Zero-invention control: one sentence per frame, frames + registry only, nothing added. Score the SHORT renders against this; score the LONG renders by striking their reported additions and comparing the remainder to this.

1. In the morning, Esmeralda, the girl's mother, gave the basket of food to Maria, the girl in the red hood.
2. She warned Maria, "Stay on the path."
3. Maria, in the dark woods, met Grumple, the hungry wolf.
4. Grumple asked Maria, "Where are you going?"
5. Maria answered Grumple, "To grandmother's cottage."
6. At the cottage, Grumple swallowed Monique, the sick grandmother.
7. In bed, Grumple disguised himself as Monique.
8. In the afternoon, at the cottage, Maria said, "What big eyes you have."
9. Gary, the passing woodcutter, cut Grumple open at the cottage.
10. Monique emerged alive.


