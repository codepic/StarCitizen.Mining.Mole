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

# Feedback Links in Documentation

- Every markdown file referenced from the README.md must have a feedback link at the top of the file.
- The feedback link should use a 💬 message icon and the text: "Send feedback on this page".
- The link must point to the GitHub issues page for this repository, using the custom issue template `feedback.yml`.
- The link must prepopulate the issue with the file name (as both the title and in the body).
- The feedback issue template must include a required dropdown for "Feedback Type" (options: Correction, Suggestion, Question, Praise, Other) and a required free-text field for details.
- The feedback link must not be added to markdown files that are not referenced from the README.md.
- The feedback link must use regular markdown link syntax (no special styling or HTML).
- When updating, renaming, or adding markdown files referenced from the README.md, ensure the feedback links are kept up to date.
- The feedback links must use the correct GitHub repository owner and name in the URL.
- The feedback links for this repository must use `codepic` as the owner and `StarCitizen.Mining.Mole` as the repo in the URL.