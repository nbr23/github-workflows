# github-workflows
Collection of useful [reusable github](https://docs.github.com/en/actions/using-workflows/reusing-workflows) workflows

## Using reusable workflows in your projects

Either simply copy the workflow file (updating its `on` directive) to your repository, or call the workflow directly through this repository:

```yml
name: Tag pyproject bump

on:
  push:
    branches:
      - main

jobs:
  call-workflow:
    uses: nbr23/github-workflows/.github/workflows/tag-pyproject-version-bump.yml@main
```
