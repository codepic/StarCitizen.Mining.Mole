# Markdown

## headings
- Do not make links to headings.

## Mermaid Diagrams
- Do not make markdown links to Mermaid diagrams.

## Tables
- Always leave an empty line before a table to ensure proper rendering with Github Pages.

## Table of Contents in README.md
- Always ensure that the links in the Table of Contents are correct and point to the right sections in the documents.
- Top-level headings should link directly to the document without a link to a specific heading.
- Before updating the Table of Contents, ensure that the linked document has consistent heading levels and numberings.
- When generating anchor links, use GitHub's automatic anchor format: lowercase, spaces replaced with hyphens, and most punctuation removed. See: https://gist.github.com/asabaylus/3071099
- **Important:** Only apply heading numbering from the main README.md to markdown files in the root folder. Do not apply README.md numbering to markdown files in any subfolder; subfolder markdown files should use their own internal numbering as appropriate.

# Feedback Links in Documentation

- Every markdown file referenced from the README.md must have a feedback link at the very top of the file, before any headings or front matter.
- The feedback link should use a 💬 message icon and the text: "Send feedback on this page".
- The link must point to the GitHub issues page for this repository, using the custom issue template `feedback.yml`.
- The link must prepopulate the issue with the file name (as both the title and in the body).
- The feedback issue template must include a required dropdown for "Feedback Type" (options: Correction, Suggestion, Question, Praise, Other) and a required free-text field for details.
- The feedback link must not be added to markdown files that are not referenced from the README.md.
- The feedback link must use regular markdown link syntax (no special styling or HTML).
- When updating, renaming, or adding markdown files referenced from the README.md, ensure the feedback links are kept up to date.
- The feedback links must use the correct GitHub repository owner and name in the URL.
- The feedback links for this repository must use `codepic` as the owner and `StarCitizen.Mining.Mole` as the repo in the URL.
- **Example:**
  `[💬 Send feedback on this page](https://github.com/codepic/StarCitizen.Mining.Mole/issues/new?template=feedback.yml&title=Feedback+on+BaseSetup.md&page=BaseSetup.md)`

# Validating TOC and Heading Consistency in Documentation

## Purpose
Manual process for ensuring the Table of Contents (TOC) in `README.md` and all linked markdown documents are consistent, correctly numbered, and follow feedback and title casing requirements.

---

## 1. Validate TOC Top-Level Numbering
- Review the TOC in `README.md`.
- Ensure each top-level entry (e.g., `1.`, `2.`, `3.`) is numbered sequentially, with no gaps or duplicates.
- Example:

```
- [1. Base Setup](BaseSetup.md)
- [2. Mining Location Selection](MiningLocation.md)
- [3. Radar Mechanics](RadarMechanics.md)
```

---

## 2. Validate H1 Headings in Linked Documents
- For each markdown file linked at the top level in the TOC:
  - **Only apply the TOC number to markdown files in the root folder.** Do not apply README.md numbering to markdown files in any subfolder; subfolder markdown files should use their own internal numbering as appropriate.
  - The H1 heading (`#`) must match the TOC number (e.g., `# 1. Base Setup`).
  - The heading text should follow generally accepted title casing rules. (Recommended: [AP Title Case](https://titlecase.com/) or [Chicago Manual of Style](https://www.chicagomanualofstyle.org/tools_citationguide/citation-guide-1.html))
  - If the H1 heading is missing, add it. If the number or text is inconsistent, update it to match the TOC number and the document’s intended title.

---

## 3. Validate and Fix Heading Numbering Within Each Document
- For each linked markdown file:
  - **Only apply the README.md numbering sequence to markdown files in the root folder.** For markdown files in subfolders, use their own internal numbering as appropriate, not the README.md sequence.
  - All numbered headings (e.g., `1.1`, `2.3.1`) must be sequential, with no gaps or duplicates.
  - If a heading is not numbered but should be, add the correct number.
  - If numbering is out of order, renumber all subsequent headings to restore sequential order.
  - Heading text should use title case.
  - When headings contain special characters (e.g., &, /, (), etc.), ensure anchor links are generated according to GitHub's anchor rules (see above).
  - Example:
    ```markdown
    ## 2.1 Factors Influencing Mining Location Choice
    ### 2.1.1 Miner Type
    ### 2.1.2 Skill Level
    ```

---

## 4. Validate and Update TOC Links for Subheadings
- Once all documents are consistent:
  - Update the TOC in `README.md` so that all second-level and deeper links (e.g., `1.1`, `2.3.1`) match the actual headings and anchor links in the documents.
  - H1 links should point to the document only (e.g., `BaseSetup.md`).
  - H2/H3 links should use the correct anchor format (e.g., `BaseSetup.md#11-turret-loadout-overview`).
  - Ensure anchor links are technically valid (no unsupported special characters, correct casing, etc.).

---

## 5. Cross-Document Link Validation
- For all cross-document links in the linked markdown files:
  - Check that the target file and anchor exist and are valid.
  - Update links if the heading or anchor has changed.

---

## 6. Feedback Link Verification
- At the top of each markdown file referenced from the TOC:
  - Ensure there is a feedback link in the following format, as the first content in the file:
    ```markdown
    [💬 Send feedback on this page](https://github.com/codepic/StarCitizen.Mining.Mole/issues/new?template=feedback.yml&title=Feedback+on+<FILENAME>&page=<FILENAME>)
    ```
  - The link must use the correct file name and repository owner/name.
  - If missing or incorrect, add or update it.

---

## 7. Ignore Non-TOC Files
- Do not check or update markdown files not referenced in the TOC.

---

## 8. General Notes
- Always use generally accepted title casing for all headings (see style guide links above).
- When in doubt, follow the document’s internal structure for subheading levels, but ensure numbering is always sequential and matches the TOC hierarchy.
- Use examples in your commit messages or documentation updates to clarify changes.
- If any steps can be automated (e.g., checking for feedback links, validating anchor links), note which are best done by script and which require human review.
- Use descriptive commit messages for documentation changes, especially when renumbering or updating anchors, to aid future audits.

---

## Section Structure: References & Related Guides

Where relevant, each documentation page should end with the following two sections, using the next sequential heading number, and always in this order:

1. `n.n References & Further Reading`
2. `n.n Related Guides`

The `References & Further Reading` section must always come before the `Related Guides` section when both are present.

---

## n.n References & Further Reading

This section contains all the external links mentioned on the page. It may also include additional links to community content.

## n.n Related Guides

Cross-linking between related guides in this repository.

---

All headings must follow the heading and numbering rules described elsewhere in this documentation.

---

## Example Commit Message
```
Validate and fix TOC and heading numbering for BaseSetup.md and MiningLocation.md. Ensured sequential numbering, correct title casing, and updated feedback links.
```
