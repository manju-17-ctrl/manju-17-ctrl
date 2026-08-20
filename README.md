name: Generate Snake Animation

on:
  schedule:
    - cron: "0 0 * * *"    # runs once a day
  workflow_dispatch: {}      # lets you trigger it manually
  push:
    branches:
      - main

jobs:
  generate:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    steps:
      - name: Generate the snake game from GitHub contribution grid
        uses: Platane/snk@v3
        with:
          github_user_name: manju-17-ctrl
          outputs: |
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
            dist/github-contribution-grid-snake.svg

      - name: Push output to the output branch
        uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

💻 GitHub: "@manju-17-ctrl" (https://github.com/manju-17-ctrl)

---

⭐ Thank You for Visiting!

Feel free to explore my repositories and projects.

⭐ If you find something interesting, consider giving it a star!
