# Naming Conventions

Consistent names make the Platform Engineer Blueprint easier to navigate, review, and maintain. These conventions apply to repository content created under [Blueprint v0.1](BLUEPRINT-v0.1.md).

## Files

- Use lowercase names with hyphen-separated words.
- Use `.md` for Markdown documents.
- Use stable, descriptive names that reflect the document's purpose.
- Use numeric prefixes for ordered content: `01-source-control-basics.md`.
- Avoid spaces, underscores, dates, temporary labels, and status words such as `draft`, `final`, or `new`.
- Use template filenames that identify the content type: `lesson-template.md`, `lab-template.md`.

## Directories

- Use lowercase names with hyphen-separated words.
- Use two-digit numeric prefixes for ordered chapter directories.
- Match chapter directory names to the canonical chapter index where possible.
- Keep directory names stable after publication because internal links depend on them.
- Place reusable authoring assets under `templates/` and durable standards under `docs/`.

## Lessons

- Use two-digit lesson numbers inside chapter directories.
- Use filenames that describe the lesson concept rather than the tool used in an example.
- Use the document title to state the lesson topic clearly.
- Align each lesson with exactly one primary Blueprint v0.1 chapter.
- Use the standard lesson structure in [lesson-template.md](../templates/lesson-template.md).

## Labs

- Use filenames that begin with the related lesson number when the lab belongs to a lesson.
- Include `lab` in the filename when the file is primarily hands-on: `03-build-artifact-lab.md`.
- Name labs after the outcome the learner validates.
- Keep lab names independent of private environments or personal machine names.
- Use the standard lab structure in [lab-template.md](../templates/lab-template.md).

## Diagrams

- Prefer Mermaid diagrams embedded in the Markdown file they support.
- Use separate diagram files only when reuse or size makes embedding impractical.
- Name standalone diagram files after the system, flow, or concept shown.
- Use lowercase hyphenated names for standalone diagram files.
- Keep diagram labels short, stable, and consistent with surrounding text.

## Branches

- Use descriptive branch names with a type prefix.
- Use `feature/` for new documentation structures, templates, or major additions.
- Use `docs/` for documentation-only refinements.
- Use `fix/` for corrections.
- Use `chore/` for repository maintenance.
- Use lowercase hyphenated topics after the prefix.

## Pull Requests

- Use clear titles that describe the reviewable change.
- Include the version or scope when the change establishes repository standards.
- Keep pull requests focused on one topic.
- Describe whether the pull request introduces learning content, repository structure, standards, or maintenance changes.
- Mention important files changed and the reason for the change.

## Commit messages

- Use imperative mood: `Add repository templates and authoring standards`.
- Keep the first line concise and specific.
- Capitalize the first word.
- Do not end the subject line with a period.
- Avoid vague subjects such as `Updates`, `Fixes`, or `Changes`.
- Make the subject read naturally after `This commit will`.
