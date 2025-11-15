# GitHub Actions Workflows

## Snake Animation Workflow

The `snake.yml` workflow generates an animated snake that "eats" your GitHub contribution graph squares.

### How It Works

1. **Schedule**: The workflow runs automatically every 24 hours to keep the animation up-to-date with your latest contributions.

2. **Manual Trigger**: You can manually trigger the workflow from the Actions tab in GitHub by clicking "Run workflow".

3. **Automatic Updates**: The workflow also runs on every push to the main branch.

4. **Output**: The generated snake animation is pushed to the `output` branch and is accessible at:
   - Light theme: `https://raw.githubusercontent.com/AnishRoy50/AnishRoy50/output/github-contribution-grid-snake.svg`
   - Dark theme: `https://raw.githubusercontent.com/AnishRoy50/AnishRoy50/output/github-contribution-grid-snake-dark.svg`

### Technology

- Uses [Platane/snk](https://github.com/Platane/snk) to generate the snake animation
- Uses [crazy-max/ghaction-github-pages](https://github.com/crazy-max/ghaction-github-pages) to push the output to a branch

### Permissions

The workflow requires `contents: write` permission to push the generated files to the `output` branch.
