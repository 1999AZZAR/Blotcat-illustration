# QA Checklist

## Must Pass

- Is it a 16:9 horizontal format?
- Is the background clean, pure white?
- Is Blotcat present?
- Does Blotcat perform the core action, rather than just being a decoration?
- Is a new metaphor generated for the current article, rather than copying past examples?
- Is the visual quirky, creative, and interesting?
- Is it simple and clean, with the main subject taking up no more than ~60% of the canvas?
- Does one image explain only one core structure?
- Are the text annotations sparse, short, and legible?
- Is orange used only for the main path or arrows?
- Is red used only for emphasis, problems, reminders, or results?
- Is blue used only for supplementary explanations, feedback, or system state?

## Failure Signals

If any of the following occur, regenerate or locally edit:

- Top-left corner has titles like "Common Pitfalls / Workflow / System Architecture / Roadmap".
- Blotcat looks like a mascot, meme, or cute cartoon.
- The image looks like a PPT, course slide, or formal flowchart.
- Too many elements, too many arrows, too many nodes.
- Text turns into long paragraphs of explanation.
- Background has paper texture, shadows, gradients, beige color, or noise.
- Looks like real UI screenshots or high-tech interfaces.
- Severe typos or illegible annotations.
- The visual is too rigid and lacks an absurd metaphor.
- Too similar to the composition of past examples in `assets/examples/`.

## Iteration Methods

- Too generic: Make Blotcat the subject of the action, add a strange but plausible metaphor.
- Too complex: Delete nodes, keep only one action and 3-5 short annotations.
- Too cute: Emphasize "deadpan, blank serious expression, not cute, not mascot".
- Too PPT-like: Remove titles, borders, neat grids, and excessive arrows; change to a hand-drawn scene.
- Too similar to old examples: Keep the core meaning but change the main object and Blotcat's action.
- Text errors: Prioritize local edits; if there are many errors, regenerate and reduce the number of annotations.

## Delivery Standard

A high-quality image should make the reader feel it's "a bit weird" at first glance, but understand the structure within 1 second.

If it looks like a tutorial slide at first glance, instead of a quirky product sketch on white paper, it fails.
