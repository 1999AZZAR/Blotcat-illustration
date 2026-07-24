# Blotcat Quirky Body Illustrations

Generate 16:9 horizontal body text illustrations for English articles. Turns key judgments, workflows, structures, states, and metaphors into clean, hand-drawn explanatory images featuring **Blotcat** — a deadpan solid-black cat who seriously performs absurd but valid tasks.

## Visual Identity

- **Blotcat**: Solid-black cat, white dot eyes, pointed ears, stick limbs. Always the core action subject — never a decoration.
- **Style**: Pure white background, black hand-drawn line art (slightly wobbly), abundant white space (~35%+), sparse handwritten English annotations in red/orange/blue.
- **Format**: 16:9 horizontal, one structure per image.
- **Color logic**: Black (main line art), orange (flow/paths/arrows), red (warnings/problems/results), blue (supplementary notes/system state).
- **No**: PPT infographics, flowcharts, cute cartoons, commercial illustrations, gradients, shadows, textures, or top-left titles.

## Usage

Invoke via `$blotcat-illustrations` in any agent prompt.

### Shot List Only (Strategy-First)

```text
Use $blotcat-illustrations do not generate images yet.
Please analyze where this article is worth illustrating, and output a shot list of about 5 images.
For each image clearly write:
- After which paragraph it is placed
- Theme of the image
- Core meaning
- Structure type
- What Blotcat is doing in the image
- Suggested elements
- Suggested English annotation words

<Paste article>
```

### Generate Full Article Illustrations

```text
Use $blotcat-illustrations to generate 4 Blotcat quirky body text illustrations for the following article.
Requirements: 16:9 horizontal, pure white background, black hand-drawn line art, sparse red/orange/blue handwritten English annotations.
Each image should only explain one core structure, no PPT infographics, no cute cartoons.

<Paste article>
```

### Single Idea Illustration

```text
Use $blotcat-illustrations to generate a 16:9 body text illustration for this viewpoint:

Trust is not shouted out, but paved piece by piece with evidence.

The visual should be quirky but clean, Blotcat must perform the core action.
English annotations at most 5, keep them short.
```

### Edit Existing Image

```text
Use $blotcat-illustrations to help me edit this image.
Remove the "Workflow / Flowchart" title and underline in the top left corner, keep other content unchanged.
Do not add any new text or objects.
```

## Structure Types

Choose one per image. Do not mix.

| Type | Use Case |
|---|---|
| **Workflow** | Input → Processing → Output, AI workflows, automation chains |
| **System Partial** | Information sources, filters, databases, agent components |
| **Before & After** | Chaos/Order, Manual/Automatic, Anxiety/Stability |
| **Character State** | User pain points, tool overload, information anxiety |
| **Conceptual Metaphor** | Content factories, information warehouses, brain black boxes |
| **Method Layering** | Methodology frameworks, skill stacks, content system layers |
| **Map Route** | Idea to launch, user paths, handoff paths, learning roadmaps |
| **Comic Panels** | Failure to success, real processes, before/after use |

## Example Images

Located in `assets/examples/`. These exist for style calibration only — do not copy compositions directly.

| File | Theme |
|---|---|
| `01-information-overload.png` | Information Overload — Blotcat buried under streams of data |
| `02-manual-vs-automation.png` | Manual vs Automation — before/after comparison |
| `03-product-journey.png` | Product Journey — map route from idea to launch |
| `04-content-factory.png` | Content Factory — conceptual metaphor for content operations |
| `05-two-breakpoints.png` | Two Breakpoints — workflow with failure points |
| `06-minimum-loop.png` | Minimum Loop — tight feedback cycle |
| `07-sort-by-purpose.png` | Sort by Purpose — method layering / categorization |
| `08-one-fish.png` | One Fish, Many Uses — single input, multiple outputs |
| `09-handoff-path.png` | Handoff Path — map route between teams or stages |
| `10-three-sources.png` | Three Information Sources — system partial composition |
| `11-common-pits.png` | Common Pitfalls — Blotcat warning at a trap-filled path |
| `12-feedback-loop.png` | Feedback Loop — cyclic workflow |
| `13-depth-vs-breadth.png` | Depth vs Breadth — before/after or comparative structure |
| `14-single-source.png` | Single Source of Truth — central system node |
| `15-bottleneck.png` | Bottleneck — congestion in a pipeline |
| `16-version-control.png` | Version Control — branching paths or versions |
| `17-context-switch.png` | Context Switch — character state, multitasking pain |
| `18-compound-growth.png` | Compound Growth — escalating returns over time |
| `19-signal-vs-noise.png` | Signal vs Noise — filtering relevant from irrelevant |
| `20-the-last-mile.png` | The Last Mile — final delivery or completion gap |

See `assets/examples/prompts.md` for reusable invocation examples.

## Character Sheets

Located in `assets/character-sheets/`. These are optional character-consistency references, not article illustration examples.

| File | Calibration Use |
|---|---|
| `operator_action.png` | Actions and movement |
| `operator_duty.png` | Operator roles and duties |
| `operator_expression.png` | Deadpan facial expression |
| `operator_pose.png` | Silhouette and poses |

Consult only the relevant sheet when needed. Do not copy sheet layouts, labels, or pose grids into generated article illustrations.

## Quality Checklist

Before delivering, verify:

- [ ] 16:9 horizontal, pure white background
- [ ] Blotcat performs the core action (not decoration)
- [ ] New metaphor for this article (not copied from examples)
- [ ] Subject occupies ~40-60% of canvas, >=35% white space
- [ ] One image = one core structure
- [ ] Target 3-5 short handwritten labels; never exceed 8
- [ ] No top-left title like "Workflow / System Architecture"
- [ ] Not PPT-like, not a formal flowchart, not cute
- [ ] Orange for flow only, red for problems/results, blue for notes

Failing any of these: regenerate or locally edit.

## Iteration Guide

| Problem | Fix |
|---|---|
| Too generic | Make Blotcat the action subject; add a strange but valid metaphor |
| Too complex | Delete nodes; keep one action and 3-5 annotations |
| Too cute | Emphasize deadpan, blank expression, not mascot-like |
| Too PPT-like | Remove titles, borders, neat grids, excessive arrows |
| Too similar to examples | Keep meaning, change main object and Blotcat's action |
| Text errors | Locally edit, or regenerate with fewer labels |

## Project Structure

```
assets/examples/     # Style calibration images + prompts.md
assets/character-sheets/ # Optional Blotcat character calibration
references/          # Style DNA, Blotcat IP, composition patterns, prompt template, QA checklist
agents/openai.yaml   # Agent skill definition
SKILL.md             # Full workflow instructions
```

## Usage as Agent Skill

Invoke with `$blotcat-illustrations` in any prompt when the skill is installed and registered in the agent's available skills list.

## License

Internal tooling. Not for redistribution.
