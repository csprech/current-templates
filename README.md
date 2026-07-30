# Current templates

Starter and community workflows for [Current](https://github.com/csprech/current) — the open-source visual workspace for AI media workflows.

Every file in `templates/` is an ordinary Current shareable export: a workflow JSON with its typed `templateInterface` embedded, media-stripped so it opens fresh. Browse them from inside the app (**Templates** on the projects screen), or import any file straight onto a canvas.

## The starter set

| Template | Shows off |
| --- | --- |
| **Style × subject matrix** | Two batch lists cross into one prompt template — six images in one run, with the fullscreen matrix view to compare them |
| **Poster, composed** | The Layer Editor: stack images and type, feed the flattened frame to a generator |
| **Inpaint anything** | The annotation Mask tool riding its own wire into a generator's Mask input |
| **Sketch to render, locally** | On-device Canny edges steering a local ComfyUI checkpoint through the Control input — $0 in API fees |
| **Page-by-page digest** | The Document node fanning a PDF's pages out to a language model, one run per page |
| **A workflow inside a node** | The Workflow node: a saved pipeline as a single step, cost known up front |
| **Art director** | An LLM with web search researching the trend and writing the image prompt |
| **Still to motion** | One prompt driving image generation, then video generation from that frame |

## Publishing your own

1. Export your workflow from Current (**Share** produces the right file).
2. Add the JSON under `templates/` and an entry to `index.json` (`id`, `name`, `author`, `file`, plus `description`/`tags`/`nodeCount` if you like).
3. Open a pull request — the PR queue is the review queue.

The app reads this repository over `raw.githubusercontent.com`. Point `COMMUNITY_TEMPLATES_REPO` at your own `owner/repo` (or `owner/repo@branch`) to run a different marketplace.
