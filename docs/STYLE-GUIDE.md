# Style Guide

This guide defines the writing standards for the Platform Engineer Blueprint. All future lessons, chapter files, diagrams, labs, glossary entries, interview material, and engineering stories should follow these conventions while remaining aligned with [Blueprint v0.1](BLUEPRINT-v0.1.md).

## Markdown conventions

- Use GitHub Markdown only.
- Use one top-level `#` heading per document.
- Keep documents readable directly on GitHub without requiring generated site tooling.
- Use relative links for repository files.
- Prefer clear prose over dense shorthand.
- Explain acronyms on first use unless they are already defined in the same document.
- Keep content publication-ready; do not commit draft notes, unresolved comments, or incomplete sections.
- Prefer durable concepts, production behavior, and tradeoffs over vendor-specific marketing language.

## Heading hierarchy

- Start every document with a single `#` heading that names the page.
- Use `##` for major sections and `###` for subsections.
- Do not skip heading levels.
- Use sentence-style headings for explanatory content.
- Use title case only for proper nouns, file titles, and established Blueprint chapter names.
- Keep headings concise enough to scan in a rendered table of contents.

## Lists

- Use unordered lists for related guidance, examples, benefits, risks, and takeaways.
- Use ordered lists for workflows where sequence matters.
- Keep list items parallel in structure when possible.
- Avoid deeply nested lists; convert complex nested lists into subsections or tables.
- End complete-sentence list items with periods.
- Keep short fragment list items punctuation-free unless consistency requires punctuation.

## Tables

- Use tables for compact reference material, indexes, comparisons, and conventions.
- Keep table columns narrow enough to render well on GitHub.
- Use descriptive column names.
- Avoid putting long paragraphs inside table cells.
- Prefer prose sections when the content needs explanation, nuance, or examples.

## Mermaid diagrams

- Use fenced `mermaid` code blocks for diagrams.
- Prefer simple `flowchart` diagrams for learning paths, request flows, ownership boundaries, and feedback loops.
- Keep node labels short and readable.
- Explain the purpose of each diagram in surrounding prose.
- Keep diagrams synchronized with the written explanation.
- Avoid diagrams that duplicate nearby text without adding clarity.
- Use Mermaid only when it improves understanding in GitHub's renderer.

## Callouts

Use blockquotes for short callouts that deserve emphasis.

> Key idea: a platform abstraction should reduce cognitive load without hiding operational responsibility.

Callouts should be brief and should not replace the main explanation. Use plain labels such as `Key idea`, `Production note`, `Security note`, or `Interview lens` at the start of the blockquote when a label improves scanning.

## Code blocks

- Use fenced code blocks.
- Include a language identifier when the language is known.
- Use `text` for shell output, file trees, logs, and plain terminal transcripts.
- Use `bash` for shell commands.
- Keep examples minimal and focused on the concept being taught.
- Explain commands before or after the block so learners understand why they are running them.
- Do not include secrets, real credentials, or environment-specific private values.

## File naming

- Use lowercase filenames.
- Separate words with hyphens.
- Use `.md` for Markdown documents.
- Use numeric prefixes for ordered chapter and lesson material.
- Keep names descriptive and stable.
- Avoid spaces, underscores, and ambiguous abbreviations.
- Follow the detailed rules in [Naming Conventions](NAMING-CONVENTIONS.md).

## Cross-references

- Use relative links for all repository references.
- Link to [Blueprint v0.1](BLUEPRINT-v0.1.md) when explaining chapter scope.
- Link to [System Map](SYSTEM-MAP.md) when explaining the idea-to-production flow.
- Link only when the destination adds useful context.
- Prefer stable document links over links to line numbers.
- Keep link text descriptive; avoid vague text such as `click here`.
- Update cross-references when files move or names change.
