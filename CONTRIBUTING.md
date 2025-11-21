# Contributing

Thank you for helping improve these freelancing guides. This repository uses SSH for GitHub access and CC BY-NC 4.0 for content.

## Prerequisites
- Git with SSH access to GitHub (`ssh -T git@github.com` to confirm).
- Markdown editor; optional image optimizer.

## Workflow
1. Branch from `main`: `git checkout -b article/<slug>`.
2. Add your article at `articles/<year>/<slug>.md` using the front matter template from `README.md`.
3. Store images under `articles/assets/<slug>/` and link them relatively (for example, `![alt](./assets/<slug>/diagram.png)`).
4. Update `articles/README.md` with title, date, status, and a link to the file.
5. Keep paragraphs short, prefer bullets for steps, and follow `STYLEGUIDE.md`.
6. If formatters or linters exist, run them before committing.
7. Commit and push via SSH: `git add . && git commit -m "Add article <slug>" && git push -u origin article/<slug>`.
8. Open a pull request describing the article and any assets added.

## Commit messages
- Use imperative present tense (for example, `Add article on tax registration`).
- Group related changes into a single commit when possible.

## Reviews
- Expect feedback on clarity, accuracy, structure, and compliance with the style guide.
- Respond to comments or push follow-up commits to the same branch.

## License
- By contributing, you agree that your submissions are licensed under the Creative Commons Attribution-NonCommercial 4.0 International license.
