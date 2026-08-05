# MSc AI E-Portfolio

Personal e-portfolio for the MSc in Artificial Intelligence at the University of Essex.
Static site — plain HTML/CSS/JS, no build step, hosted on GitHub Pages.

**Live site:** `https://your-username.github.io`

## Files

| File | What it is |
|---|---|
| `index.html` | Homepage — bento grid of all 8 modules, skills, and contact |
| `module-01.html` | Launch into Computing |
| `module-02.html` | Understanding Artificial Intelligence |
| `module-03.html` | Numerical Analysis |
| `module-04.html` | Intelligent Agents |
| `module-05.html` | Machine Learning |
| `module-06.html` | Knowledge Representation & Reasoning |
| `module-07.html` | Research Methods & Professional Practice |
| `module-08.html` | MSc Computing Project |

Each module page is self-contained (its own `<style>` and `<script>`), so you can edit one without touching the others.

## How to edit

All editing happens in the GitHub web editor: open a file → pencil icon (top right) → make changes → commit. The live site updates within a minute or two.

**Change a module's status** (e.g. mark Module 4 as completed):
- On `index.html`, find that module's card and change `<span class="tab progress">In progress</span>` to `<span class="tab done">Completed</span>`
- On the module's own page, do the same for `<span class="status-badge progress">`

**Write the module overview:**
- Open the module's page, find the `/ Overview` section, replace the placeholder text inside the `<p>` tag in the `.panel` div

**Add files to a module:**
- Copy the actual file (PDF, code, dataset) into the repo, in the same folder as the HTML files
- In the module's page, find the `/ Files` section and add a new `.file-row` block (copy an existing one as a template), updating the file name and size
- Wrap the file name in a link (`<a href="your-file.pdf">...</a>`) so it's actually downloadable

**Add a 9th module:**
- Duplicate any `module-0X.html`, rename it, update its title/number/content
- Add a matching card on `index.html` linking to it
- Add it to the small circular module-nav list at the top of every module page

## Design notes

- Palette: deep violet background, coral / gold / teal accents
- Fonts: Space Grotesk (headings), Manrope (body), JetBrains Mono (labels/data)
- Animated wavy background + "crash-landing" entrance animation on scroll, on every page
