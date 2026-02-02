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

1. When you push to `main`, the workflow:
   - Compiles the Quarto presentation to HTML
   - Deploys the output to the `gh-pages` branch

2. The generated HTML files are **not** tracked in source control (see `.gitignore`), keeping the repository small and the single source of truth in the `.qmd` files.

### Setup for your fork

1. Go to your repository's **Settings** → **Pages**
2. Under **Build and deployment**, set:
   - **Source**: `Deploy from a branch`
   - **Branch**: `gh-pages` / `/ (root)`
3. Click **Save**
4. Push a commit to trigger the workflow, or manually run it via **Actions** → **Build and Deploy Presentation** → **Run workflow**
5. Your presentation will be available at `https://<username>.github.io/<repo-name>/`

## Disclaimer

Ask for permission before using your phone to control the presentation in an exam.