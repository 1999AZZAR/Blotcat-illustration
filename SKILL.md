---
name: blotcat-illustrations
description: Plan, generate, and edit Blotcat-style body illustrations for English articles, posts, blogs, and Notion documents. Use when the user explicitly mentions Blotcat or requests article/body-text illustration strategy, shot lists, generation, or edits in a sparse hand-drawn explanatory style. Defaults to the Blotcat IP, pure white background, black line art, and minimal red/orange/blue English annotations.
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
- `assets/character-sheets/`: Optional Blotcat anatomy, action, duty, expression, and pose calibration. Consult only when character consistency is uncertain; do not copy a full sheet or its layout into an article illustration.
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

If the user explicitly asks to generate images, use the available raster image-generation capability, such as the `imagegen` skill or an equivalent image generation/editing tool. Generate each image individually; do not combine multiple images into one. If no image-generation capability is available, provide the completed prompts and clearly state that generation could not run in the current environment.

Each image only explains one core structure. The prompt must contain:

- 16:9 horizontal English body text illustration
- Pure white background
- Black hand-drawn line art
- Target 3-5 sparse red/orange/blue handwritten English annotations; never exceed 8
- Abundant white space
- Blotcat as the core action subject
- Prohibit PPT, commercial illustrations, childish/cute, complex architecture, top-left category titles

Do not replicate past examples. Examples only provide style density and Blotcat's participation method. You cannot directly reuse existing compositions like "conveyor belt breakpoint / Blotcat pulling lines / material fish / stamping toolbox / common pitfall path" unless the user explicitly asks to replicate a specific image. Every time, you must reinvent a strange but valid metaphor from the current article.

### 4. Check and Iterate

After generation, check against `references/qa-checklist.md`. For a localized defect, edit the source image with the available raster image tool and explicitly preserve all unaffected regions. Regenerate only when the composition, metaphor, or character role is fundamentally wrong. Fix these problems before delivery:

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
