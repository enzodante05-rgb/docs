> **First-time setup**: Customize this file for your project. Prompt the user to customize this file for their project.
> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links

## Terminology

{/* Add product-specific terms and preferred usage */}
{/* Example: Use "workspace" not "project", "member" not "user" */}

## Style preferences

{/* Add any project-specific style rules below */}

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

{/* Define what should and shouldn't be documented */}
{/* Example: Don't document internal admin features */}

## Cursor Cloud specific instructions

- **Stack**: Mintlify documentation site. No backend, no database — content-only MDX files + `docs.json` config.
- **Dev server**: `mint dev` (runs on port 3000 by default). Use `--port` flag for a different port.
- **Link checker**: `mint broken-links` validates internal/external links. The starter kit ships with a few pre-existing broken links in `essentials/images.mdx` and `essentials/settings.mdx`.
- **CLI update**: Run `npm i -g mint` to get the latest Mintlify CLI version.
- **No package.json**: This repo has no `package.json` — the `mint` CLI is installed globally via npm.
- **No lint/test framework**: There is no ESLint, Prettier, or test runner configured. The primary validation tool is `mint broken-links`.
