---
name: blotcat-illustrations
description: Generate English body text illustrations. Used when the user requests "quirky", "Blotcat", "hand-drawn", "body text illustration", "article illustration", "illustration suggestions", "shot list", or "remove title/edit image" for English articles, posts, blogs, Notion docs, workflows, methodology, processes, structures, states, metaphors, or viewpoints; defaults to using the Blotcat IP, pure white hand-drawn style, minimal red/orange/blue annotations, and a clean but imaginative visual style.
---

# Blotcat Quirky Body Illustrations

## Core Positioning

Design and generate 16:9 horizontal body text illustrations for articles. The goal is not to create commercial illustrations, PPT infographics, or cute cartoons, but to turn the key judgments, processes, structures, states, or metaphors in the article into a clean, quirky, creative, readable but not overly instructional hand-drawn explanatory image.

The default visual IP is "Blotcat": a solid black, white-dot-eyed, thin-legged, blank-expression creature seriously doing something absurd but valid. Blotcat must participate in the core action of the image, not just stand aside as a decoration.

## Read These References First

Read them as needed for the task, do not cram everything into the context at once:

- `references/style-dna.md`: Style DNA, colors, text, taboos.
- `references/blotcat-ip.md`: Blotcat IP's appearance, personality, action library, and taboos.
- `references/composition-patterns.md`: Structure types, original metaphor methods, and anti-copying rules.
- `references/prompt-template.md`: Single image generation prompt template.
- `references/qa-checklist.md`: Post-generation inspection and iteration rules.
- `assets/examples/`: Only for low-frequency visual calibration, do not enter the default generation path. Do not copy the compositions, objects, or annotations of these examples.

## Workflow

### 1. Digest the Main Text

First, read the main text, link, Notion page, Markdown file, or screenshot content provided by the user. Extract:

- What is the core viewpoint
- Which paragraphs carry cognitive transitions
- What content is suitable for visual explanation
- Where is only suitable for text and doesn't need images

Do not illustrate evenly. Prioritize "cognitive anchors", for example: core judgments, two breakpoints, input-output loops, branching, before-and-after comparisons, one-fish-many-uses, handoff paths, common pitfalls, character state changes.

### 2. Provide Illustration Strategy First

If the user just says "analyze how to illustrate / think about where illustrations are needed", provide a shot list first. For each image clearly write:

- After which paragraph it is placed
- Theme of the image
- Core meaning
- Structure type
- What Blotcat is doing in the image
- Suggested elements
- Suggested English annotation words

Default to 4-8 images. 1-3 images for short articles; do not easily exceed 9 images even for long articles. Just enough is good, avoid turning the article into a picture book.

### 3. Generate Single Images

If the user explicitly asks to "generate / output / make images / help me generate", do not stop and wait for confirmation; use the built-in `image_gen` to generate each image individually. Do not combine multiple images into one.

Each image only explains one core structure. The prompt must contain:

- 16:9 horizontal English body text illustration
- Pure white background
- Black hand-drawn line art
- Sparse red/orange/blue handwritten English annotations
- Abundant white space
- Blotcat as the core action subject
- Prohibit PPT, commercial illustrations, childish/cute, complex architecture, top-left category titles

Do not replicate past examples. Examples only provide style density and Blotcat's participation method. You cannot directly reuse existing compositions like "conveyor belt breakpoint / Blotcat pulling lines / material fish / stamping toolbox / common pitfall path" unless the user explicitly asks to replicate a specific image. Every time, you must reinvent a strange but valid metaphor from the current article.

### 4. Check and Iterate

After generation, check against `references/qa-checklist.md`. If the following problems occur, prioritize regenerating or local editing:

- Blotcat is just a decoration
- The image is too full
- Looks too much like a flowchart/PPT
- Too much English or severe typos
- Titles like "Common Pitfall/Flowchart/System Architecture" appear in the top-left corner
- Art style is too cute, childish, or rigid
- Background is not a clean white

### 5. Save and Deliver

If the user is working within a workspace, copy the final images to:

```text
assets/<article-slug>-illustrations/
```

Name them sequentially:

```text
01-topic-name.png
02-topic-name.png
```

Keep the original generated files, do not overwrite existing assets unless explicitly requested by the user.

## Output Tone

Pre-generation strategy output should be short and precise. Post-generation delivery should include:

- How many images were generated
- The purpose of each image
- Save paths
- Which images are the most solid, which are optional

Do not give long explanations of style theory; let the images speak for themselves.
