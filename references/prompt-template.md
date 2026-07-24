# Image Generation Prompt Template

Generate each image individually. Replace variables based on the article's content, do not combine multiple images into one.

```text
Generate one standalone 16:9 horizontal English article illustration.

Visual DNA:
Pure white background. Minimalist black hand-drawn line art. Slightly wobbly pen lines. Lots of empty white space. Sparse red/orange/blue handwritten English annotations. Clean absurd product-sketch feeling. No gradients, no shadows, no paper texture, no complex background, no commercial vector style, no PPT infographic look, no cute mascot poster, no children's illustration, no realistic UI.

Recurring IP character required:
Blotcat, a small minimalist solid-black cat with white dot eyes, two subtle pointed ears, tiny stick-like legs and arms, and a simple bean-like cat shape. Blotcat must perform the core conceptual action, not decorate the scene. Make Blotcat serious, deadpan, and slightly bizarre, not cute.

Theme:
{Illustration Theme}

Structure type:
{Structure Type: Workflow / System Partial / Before & After / Character State / Conceptual Metaphor / Method Layering / Map Route / Comic Panels}

Core idea:
{The core meaning this image should express}

Composition:
{Specific scene: Where is Blotcat, what is it doing, what are the main objects, how does information flow}

Suggested elements:
{Element 1} / {Element 2} / {Element 3} / {Element 4}

English handwritten labels:
{Label 1} / {Label 2} / {Label 3} / {Label 4} / {Optional Label 5}

Color use:
Black for main line art and Blotcat. Orange for main flow/path/arrows. Red only for key warnings/problems/results. Blue only for secondary notes or feedback/system state.

Constraints:
One image explains only one core structure. Keep the main subject around 40%-60% of the canvas. Preserve at least 35% blank white space. Target 3-5 short handwritten English labels, with 8 as a hard maximum. Do not write a title in the top-left corner. Do not write the structure type on the image. Do not make it a formal diagram, course slide, or dense explainer. Do not copy prior examples or reuse known case compositions unless explicitly requested; invent a fresh visual metaphor for this specific article. It should be clear but not instructional, interesting but not childish, strange but clean.
```

## Image Editing Prompts

Remove the top-left title:

```text
Edit the provided image. Remove only the handwritten title "{Text to delete}" and its underline from the top-left corner. Fill that area with the same clean white background, matching the surrounding blank paper. Preserve everything else exactly: characters, labels, paths, line style, composition, aspect ratio, and image quality. Do not add any new text or objects.
```

Enhance the sense of absurdity:

```text
Regenerate this illustration with the same core meaning and simple layout, but make Blotcat more central to the conceptual action. Blotcat should be doing the strange work that explains the idea, not standing beside the diagram. Keep it clean, sparse, hand-drawn, and not cute.
```
