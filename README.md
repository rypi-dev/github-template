# github-template
🚀 GitHub template to provide a pre-designed architecture for all types of projects.

## Intro

The purpose of this project is to provide a template for creating projects on GitHub. We use a bunch of tech to build the template, including [Commitizen](https://commitizen-tools.github.io/commitizen/), [CommitLint](https://commitlint.js.org/), [Husky](https://typicode.github.io/husky/), [BunJS](https://bun.sh/) and [GitHub Actions](https://docs.github.com/en/actions).

## Docs

To start using the project, you can [use the template](https://github.com/new?template_name=github-template&template_owner=rypi-dev) directly.

Then, follow this step-by-step guide to use our framework.

### Commitizen & CommitLint

```
# Installing dependencies
gfavreau@DESKTOP-LHPH7R7:~/github-template$ bun i
```

Add any file to your new project

```
# Add files to the commit
gfavreau@DESKTOP-LHPH7R7:~/github-template$ git add .
```

```
# Use CommitLint and Commitizen
gfavreau@DESKTOP-LHPH7R7:~/github-template$ bun git-cz
```

Well done! You've written a great commit using our first utility, and you can now send it to GitHub.

### GitHub Actions

Now, we're going to take a look at GitHub Actions. In order to use our workflows, we're going to [create GitHub apps](https://docs.github.com/fr/apps/creating-github-apps).

Next, please refer to this [documentation](https://github.com/peter-murray/workflow-application-token-action) for creating the GitHub Apps needed for the workflows.

```
# Compress Img Bots
secrets.ID_COMPRESSIMGBOT
secrets.PEM_COMPRESSIMGBOT
```

```
# Create Labels Bots
secrets.ID_CREATELABELBOT
secrets.PEM_CREATELABELBOT
```

```
# Create GitLeaks Bots
secrets.ID_GITLEAKSBOT
secrets.PEM_GITLEAKSBOT
```

## Structure

```bash
.
├── .github/                      
│   ├── .husky/                   # Husky scripts
│   ├── assets/                   # Project assets
│   ├── config/                   # Configuration des flux de travail
│   └── ISSUE_TEMPLATE/           # GitHub issue templates
│   └── workflows/                # GitHub Actions
├── LICENSES/                     # Project licences
├── .commitlintrc.js              # Configuring commitlint
├── .editorconfig                 # Editor configuration
├── .gitconfig                    # Configuring Git
```