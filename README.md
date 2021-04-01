# Community Template Repo

Template repo with docs and GitHub Actions etc, to create other projects.

##  Links :
- Discord Channel - [Join](https://discord.gg/gWwTMbuX)

## Usage

```yaml
name: Import open source standard labels

on:
  push:
    branches: [ main ]

jobs:
  labels:

    runs-on: ubuntu-latest

    steps:
    - uses: actions/setup-node@v2
      with:
        node-version: '14'
    - uses: EddieHubCommunity/gh-action-open-source-labels@main
      with:
        github-token: ${{ secrets.GITHUB_TOKEN }}
        owner-name: 'EddieHubCommunity'
        repository-name: 'gh-action-open-source-labels'
```

![screenshot](https://user-images.githubusercontent.com/624760/113267767-9e331c00-92ce-11eb-8e47-efb02d3c7fa2.png)
