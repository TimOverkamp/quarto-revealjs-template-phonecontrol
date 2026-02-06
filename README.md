# Quarto Reveal.js presentation template

This is a Quarto Reveal.js presentation template with custom phone controls using multiplex with hosting on GitHub Pages. 
**[View Presentation Template](https://timoverkamp.github.io/quarto-revealjs-template-phonecontrol/)**

## Setup

1. Clone this repository: `git clone https://github.com/timoverkamp/quarto-revealjs-template-phonecontrol.git`
2. [Install Quarto](https://quarto.org/docs/download/)
3. Run `quarto preview presentation/presentation.qmd`
4. Open `presentation.html` in your browser to view the presentation
5. Open `presentation-speaker.html` to view the speaker view, it features a timer and control buttons when you switch to scroll view (mobile, vertical) aswell as the speaker notes embedded in the slides.
6. Your presentation should now be synced with the speaker view (via multiplex). When you change slides in the speaker view, the presentation will follow.

## GitHub Pages Deployment

This template includes a GitHub Actions workflow that automatically builds and deploys your presentation to GitHub Pages.

### How it works

1. **On push to `main`**:
   - The workflow compiles the presentation and uploads it as an artifact to verify the build.
   - It does **not** deploy to GitHub Pages.

2. **On pushing a tag** (e.g. `v1.0.0`):
   - The workflow compiles the presentation.
   - It deploys the presentation to GitHub Pages.

### Setup for your fork

1. Go to your repository's **Settings** → **Pages**
2. Under **Build and deployment**, set:
   - **Source**: `GitHub Actions`
3. Click **Save**
4. To deploy, create and push a tag (must match `v*.*.*`):
   ```bash
   git tag v1.0.0
   git push origin v1.0.0
   ```
5. Your presentation will be available at `https://<username>.github.io/<repo-name>/`

## Disclaimer

Ask for permission before using your phone to control the presentation in an exam.