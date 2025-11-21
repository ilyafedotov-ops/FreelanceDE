# Markdown Style Guide

Keep articles consistent and easy to read.

## Structure
- Use a front matter block with keys ordered as: `title`, `date`, `tags`, `summary`.
- Dates in ISO format: `YYYY-MM-DD`.
- File names in kebab-case slugs: `articles/2024/register-as-freelancer.md`.
- Headings start at `#` and increase by one level; do not skip levels.

## Writing
- Use short paragraphs; prefer bullets for steps or lists.
- Keep tone clear and practical; avoid unexplained jargon.
- When citing regulations, link to official sources.
- Include a concise summary in the front matter; avoid repeating it verbatim in the intro.

## Links and assets
- Use descriptive link text (avoid bare URLs).
- Store images in `articles/assets/<slug>/` and reference them relatively: `![alt text](./assets/<slug>/diagram.png)`.
- Provide meaningful alt text for every image.

## Code and commands
- Wrap commands or code samples in fenced code blocks with a language hint (for example, ```bash```).
- Inline code uses backticks: `term`.

## Formatting
- Use ASCII characters unless a foreign term requires accents; prefer straight quotes.
- Leave a blank line between paragraphs and after headings.
- Avoid trailing whitespace.
