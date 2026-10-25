# relokv.github.io

Experimental artifacts for on-device multi-LoRA KV management.

## Contents

- `index.html`: single-column experimental materials page organized around the
  workload, setup, comparisons, metrics, ablations, and release status.
- `reproduction.html`: experiment-specific reproduction requirements.
- `data/schema.csv`: proposed field dictionary, not request data.
- `configs/environment-template.json`: metadata inventory, not a runnable
  configuration.
- `assets/`: the shared Cayman-style stylesheet and locally hosted Open Sans.

Implementations, traces, measured results,
checkpoints, and verified execution commands are not distributed in this version.
No performance or reproduction success is claimed. The site contains only
experimental materials and their documentation, with no manuscript or
architecture diagram.

The visual layout follows the supplied Cayman-style reference material sites:
a blue-to-green header, centered green paper title, badges, a plain linked
table of contents, green section headings, blue links, and unboxed single-column
prose and tables. The site is limited to experiment-related content and has no
system overview or framework diagram. Open Sans is hosted locally; its OFL
license is included in `assets/fonts/OFL.txt`. The pages require no JavaScript
or third-party network requests.

## Preview and Publishing

Open `index.html` directly in a browser. No development server, package
installation, or build step is required.

For GitHub Pages, publish from the `main` branch and `/ (root)`. Keep
`.nojekyll` at the repository root. A root user site requires the repository
name to match the owner's lowercase username plus `.github.io`.

## Updating Materials

Replace preparation states only when the linked files have actually been
published and checked. Add exact source versions, environments, run inputs,
entry points, expected outputs, and validation criteria to executable releases.
Do not invent commands or populate result tables with illustrative values.

Keep manuscripts, source TeX, private notes, credentials, personal metadata,
and raw private logs outside this repository. Check the entire public history,
commit identity, deployment activity, and downloadable files before submission.
The `.gitignore` file is only a convenience; it does not remove previously
tracked files or replace a disclosure review.
