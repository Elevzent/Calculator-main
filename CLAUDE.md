# Calculator-main Workspace Rules

## Project Shape

- This project is a single-file static H5 tool.
- The main entry is `index.html`.
- There is no build step, bundler, or framework runtime.
- New features should work by opening `index.html` directly in a browser.

## File Conventions

- Keep UI, styles, and logic in `index.html` unless the file becomes clearly unmaintainable.
- Prefer small, named helper functions over large anonymous blocks.
- Reuse existing data structures such as `inventory`, `itemDefs`, and `normalizeItemRecord()` instead of inventing parallel models.
- Record user-visible iterations in `CHANGELOG.md` under the current date before Git handoff.

## Recognition Scope

- Screenshot recognition is only for this game's backpack page.
- Do not optimize for generic game UIs or arbitrary screenshots.
- V1 recognition only extracts item shape and quality color.
- V1 does not do OCR and does not read names, numbers, or text labels from screenshots.
- Imported recognition results must be converted into the current `inventory` format and then use the existing solver flow.

## Validation

- After changes, verify behavior with a real local browser run.
- Do not add secrets, tokens, or remote services.
