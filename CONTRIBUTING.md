# Contributing to Python Documentation — Punjabi (`pa`)

Thank you for your interest in contributing to the Punjabi (Gurmukhi) translation of the Python documentation.

This project is part of the official Python Documentation Translation initiative and follows the translation workflow adopted by the Python Documentation community. Our goal is to make the official Python documentation accessible to Punjabi-speaking developers, students, educators, and the broader open-source community while maintaining the same quality standards as the upstream documentation.

Whether you are fixing a typo, translating a new document, reviewing terminology, or improving translation quality, your contributions are welcome.

---

## Contents

- [Project Status](#project-status)
- [Before You Start](#before-you-start)
- [Repository Structure](#repository-structure)
- [Translation Workflow](#translation-workflow)
- [Getting Started](#getting-started)
- [Creating New Translation Files](#creating-a-new-translation-file)
- [Validation](#validation)
- [Translation Rules](#translation-rules)
- [Quality Checklist](#quality-checklist)
- [Pull Request Guidelines](#pull-request-guidelines)
- [Commit Message Examples](#commit-message-examples)
- [Translation Standards](#translation-standards)
- [Getting Help](#getting-help)
- [References](#references)
- [License](#license)

---

# Project Status

The Punjabi (`pa`) translation project is actively maintained and follows the official Python Documentation Translation workflow.

## Project Team

The Punjabi (`pa`) translation project is maintained collaboratively by a team of coordinators and contributors through the official Python Documentation Translation project on Transifex.

### Coordinators

The project is currently coordinated by:

- Bhuvansh Kataria [@BHUVANSH855](https://github.com/BHUVANSH855)
- Mohit Yadav [@mohityadav8](https://github.com/mohityadav8)
- Yashraj Jangra [@Yashraj-Jangra](https://github.com/Yashraj-Jangra)

The coordinators are responsible for:

- Managing the translation project.
- Maintaining translation quality.
- Coordinating contributors and reviewers.
- Ensuring consistency across translated documentation.
- Overseeing validation and synchronization workflows.

---

### Current Highlights

- ✅ Officially listed in the Python Developer Guide Translation Coordinators (PR #1843)
- ✅ Active translation branch: `3.15`
- ✅ Automated synchronization with the official Python Documentation Transifex project
- ✅ GitHub Actions validation passing
- ✅ GNU gettext (`msgfmt`) validation passing
- ✅ `sphinx-lint` validation passing
- ✅ CPython HTML documentation build passing
- ✅ Nitpicky (`-n`) documentation build passing

### Completed Translation Areas

| Area | Status |
|------|--------|
| Tutorial Documentation (17/17 files) | ✅ Complete |
| Using Python Documentation (9/9 files) | ✅ Complete |
| `library/stdtypes.po` | ✅ Complete |
| `library/functions.po` | ✅ Complete |
| `library/exceptions.po` | ✅ Complete |
| `library/functools.po` | ✅ Complete |
| `library/string.po` | ✅ Complete |
| `howto/regex.po` | ✅ Complete |
| `howto/sorting.po` | ✅ Complete |
| `glossary.po` | ✅ Complete |
| `bugs.po` | ✅ Complete |

### Translation Statistics

| Metric | Value |
|--------|------:|
| Verified Translated Strings | **7,668** |
| Tutorial Files Completed | 17 |
| Using Python Files Completed | 9 |
| Core Library Files Completed | 5 |
| HOWTO Files Completed | 2 |
| Root Translation Files Completed | 2 |

### Current Priorities

Current development focuses on:

- Reviewing existing translations for terminology consistency and technical accuracy.
- Expanding translations across additional Standard Library, HOWTO, FAQ, Reference, C API, and What's New documentation.
- Maintaining consistency with `GLOSSARY.md` and `STYLE_GUIDE.md`.
- Keeping translations synchronized with upstream CPython documentation.
- Growing the Punjabi translation community and onboarding new contributors and reviewers.

---

# Before You Start

Before contributing, please ensure you have:

- A GitHub account.
- A Transifex account (recommended for translation work).
- Basic familiarity with Git and GitHub.
- Basic understanding of Python documentation and reStructuredText (RST).
- GNU gettext utilities installed (`msgfmt`, `msgattrib`, `msginit`).
- Python and Sphinx installed if you intend to perform local documentation builds.

Although many translations are performed through Transifex, contributors may also work directly with `.po` files when appropriate.

Before beginning any translation work, please read:

- `README.md`
- `STYLE_GUIDE.md`
- `GLOSSARY.md`

These documents describe the project's workflow, terminology, and translation conventions.

---

# Repository Structure

The repository is organized similarly to the upstream CPython documentation.

```text
python-docs-pa/
├── .github/              # GitHub Actions workflows
├── tutorial/             # Tutorial documentation
├── using/                # Using Python documentation
├── library/              # Standard Library documentation
├── howto/                # HOWTO guides
├── faq/                  # Frequently Asked Questions
├── reference/            # Language Reference
├── c-api/                # Python/C API documentation
├── extending/            # Extending and Embedding Python
├── installing/           # Installation documentation
├── distributing/         # Distribution documentation
├── deprecations/         # Deprecated features
├── whatsnew/             # What's New documentation
│
├── README.md
├── CONTRIBUTING.md
├── STYLE_GUIDE.md
├── GLOSSARY.md
├── PROJECT_REPORT.md
│
├── *.po                  # Root translation files
└── .gitignore
```

Each directory contains translation files (`.po`) corresponding to the official CPython documentation.

Whenever possible, contributors should work on one document or one logical translation area at a time to simplify review and maintain consistency.

# Translation Workflow

The Punjabi (`pa`) translation project follows the standard Python Documentation Translation workflow.

```text
Translate in Transifex
          ↓
Follow GLOSSARY.md
          ↓
Follow STYLE_GUIDE.md
          ↓
Peer Review
          ↓
Automated Synchronization to GitHub
          ↓
GitHub Actions Validation
          ↓
GNU gettext Validation (`msgfmt`)
          ↓
sphinx-lint
          ↓
CPython HTML Build
          ↓
Nitpicky (`-n`) Documentation Build
```

Every completed translation should successfully pass the validation pipeline before being considered ready.

---

# Getting Started

Contributors can help in several ways:

- Translate untranslated documentation.
- Review existing translations.
- Improve terminology consistency.
- Validate translations locally.
- Fix formatting or reStructuredText issues.
- Correct validation errors.
- Improve documentation quality.

For external contributors, the recommended GitHub workflow is:

1. Fork the repository.
2. Clone your fork locally.
3. Create a new branch.
4. Make your changes.
5. Validate your work.
6. Commit your changes.
7. Push the branch.
8. Open a Pull Request.

If you are translating through Transifex, translations will be synchronized automatically through the repository's GitHub Actions workflow.

---

# Creating a New Translation File

When a new CPython documentation template (`.pot`) becomes available, a corresponding Punjabi translation file can be created using GNU gettext.

Example:

```bash
msginit \
  --locale=pa \
  --input=PATH_TO_TEMPLATE.pot \
  --output-file=PATH_TO_OUTPUT.po
```

For example:

```bash
msginit \
  --locale=pa \
  --input=library/functions.pot \
  --output-file=library/functions.po
```

After creating a new `.po` file:

- Preserve the original metadata.
- Translate progressively.
- Validate frequently.
- Submit only well-tested translations.

---

# Validation

Every completed translation should pass all validation checks before submission.

> **Validation and translation review are separate processes.**
>
> Automated validation verifies translation syntax, markup preservation, and documentation build correctness. Human review focuses on terminology consistency, language quality, technical accuracy, and adherence to the project's glossary and style guide.

## Validation Pipeline

```text
Translation
      ↓
msgfmt
      ↓
sphinx-lint
      ↓
CPython HTML Build
      ↓
Nitpicky Build
```

---

## GNU gettext Validation

Check for syntax errors:

```bash
msgfmt --check FILE.po
```

Display translation statistics:

```bash
msgfmt --statistics FILE.po
```

List untranslated messages:

```bash
msgattrib --untranslated FILE.po
```

List translated messages:

```bash
msgattrib --translated FILE.po
```

---

## Documentation Validation

Run documentation linting:

```bash
sphinx-lint .
```

Build the Punjabi documentation:

```bash
python -m sphinx -b html -D language=pa Doc build/html-pa
```

Run the strict ("nitpicky") documentation build:

```bash
python -m sphinx -b html -n -W Doc build/html-pa
```

All commands should complete successfully before submitting a contribution.

---

## Review Guidelines

Review is a collaborative process intended to improve translation quality rather than simply identify errors. Contributors and reviewers are encouraged to discuss terminology, phrasing, and technical accuracy to achieve consistent, high-quality translations.

Automated validation confirms that a translation is technically valid, but it does not verify translation quality.

During review, contributors and reviewers should check:

- Technical accuracy.
- Consistency with `GLOSSARY.md`.
- Compliance with `STYLE_GUIDE.md`.
- Natural Punjabi wording.
- Preservation of reStructuredText and Sphinx markup.
- Correct handling of cross-references, directives, and code examples.

---

# Translation Rules

Maintaining consistency is one of the most important goals of this project.

Always preserve:

- Technical accuracy
- Existing terminology
- Formatting
- Documentation structure
- reStructuredText markup

---

## Never Translate

### Python Keywords

```text
if
else
elif
for
while
class
def
return
import
from
try
except
finally
raise
pass
with
yield
lambda
```

---

### Python Identifiers

Do **not** translate:

- Function names
- Class names
- Module names
- Exception names
- Variable names
- Package names

Examples:

```text
print
len
range
list
dict
tuple
set
ValueError
TypeError
KeyError
ImportError
os
sys
json
pathlib
```

---

### reStructuredText and Sphinx Markup

Never modify or translate documentation roles or directives such as:

```rst
:func:
:class:
:mod:
:meth:
:attr:
:exc:
:term:
:ref:
```

Likewise, preserve:

- Code blocks
- Inline code
- Hyperlinks
- File names
- Anchors
- Cross-references

---

### Other Items

Do not translate:

- URLs
- Python version numbers
- Command-line options
- File extensions
- Package names
- Environment variables

---

## Translate

Translate:

- Titles
- Section headings
- Paragraphs
- Explanatory text
- Notes
- Warnings
- Tips
- Comments inside code examples
- Table content
- User-facing descriptions
- Documentation narratives

Translate naturally while preserving the original meaning.

Avoid literal word-for-word translations when a more natural Punjabi expression communicates the same concept accurately.

---

## Reviewer Responsibilities

Reviewers help ensure that translations are technically accurate, linguistically natural, and consistent across the project.

A reviewer should:

- Verify terminology against `GLOSSARY.md`.
- Check compliance with `STYLE_GUIDE.md`.
- Preserve original meaning and technical intent.
- Ensure all Sphinx and reStructuredText markup remains unchanged.
- Report inconsistencies or suggest improvements through GitHub or Transifex.

---

# Quality Checklist

Before submitting your contribution, ensure that:

- [ ] All intended entries have been translated or reviewed.
- [ ] GNU gettext (`msgfmt`) validation passes.
- [ ] No reStructuredText markup has been modified accidentally.
- [ ] Code examples remain unchanged.
- [ ] Terminology follows `GLOSSARY.md`.
- [ ] Translation style follows `STYLE_GUIDE.md`.
- [ ] Translation has been reviewed for natural Punjabi wording.
- [ ] `sphinx-lint` reports no problems.
- [ ] CPython HTML documentation builds successfully.
- [ ] Nitpicky (`-n`) documentation build passes.
- [ ] GitHub Actions validation completes successfully.

# Pull Request Guidelines

Before opening a Pull Request, please ensure that your contribution is complete, focused, and ready for review.

### Before You Submit

- Sync your branch with the latest `3.15` branch.
- Keep each Pull Request focused on a single topic or documentation area whenever possible.
- Validate your translations locally before submitting.
- Ensure GitHub Actions complete successfully.
- Provide a clear description of your changes.
- Reference related issues or discussions when applicable.

Large translation efforts should be split into multiple smaller Pull Requests whenever practical to simplify review.

---

# Commit Message Examples

Use concise, descriptive commit messages.

Examples:

```text
Translate tutorial/modules.po to Punjabi

Translate library/functions.po

Translate library/stdtypes.po

Update glossary terminology

Improve translation consistency

Fix validation issues in tutorial translations

Correct formatting in reference documentation

Update Punjabi translations for Python 3.15
```

---

# Translation Standards

High-quality translations should be:

- Technically accurate.
- Natural and easy to read in Punjabi.
- Consistent with existing project terminology.
- Consistent with the official Python documentation.
- Free from grammatical and spelling errors.
- Valid according to GNU gettext and Sphinx validation tools.

Contributors should:

- Prefer natural Punjabi over literal word-for-word translations.
- Preserve the original meaning and technical intent.
- Follow the terminology defined in `GLOSSARY.md`.
- Follow the conventions described in `STYLE_GUIDE.md`.
- Preserve all reStructuredText roles, directives, hyperlinks, and formatting.
- Keep code examples identical to the original documentation.
- Preserve indentation and whitespace where required.
- Review completed translations for technical accuracy, terminology consistency, and natural Punjabi wording before submission.
- Follow translation patterns established in completed project files whenever appropriate.

When uncertain about a translation, prioritize consistency with existing project terminology rather than introducing new wording.

---

# Getting Help

If you have questions about terminology, translation style, or project workflow, consult the following project documentation first:

- `README.md`
- `STYLE_GUIDE.md`
- `GLOSSARY.md`
- `PROJECT_REPORT.md`

For project discussions, suggestions, bug reports, or translation questions, please use GitHub Issues and Pull Requests.

Constructive feedback, terminology discussions, and translation reviews are always welcome.

---

# References

Useful resources for contributors:

- **Python Developer Guide – Documentation Translations**  
  <https://devguide.python.org/documentation/translations/>

- **Python Documentation**  
  <https://docs.python.org/>

- **Python Documentation on Transifex**  
  <https://app.transifex.com/python-doc/python-newest/>

- **Python Documentation Style Guide**  
  <https://devguide.python.org/documentation/style-guide/>

- **reStructuredText Primer (Sphinx)**  
  <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>

---

# License

This project follows the licensing model of the official Python Documentation Translation project.

Documentation translations are contributed under the CC0 1.0 Universal license.

By contributing to this repository, you agree that your contributions may be distributed under the same licensing terms as the official Python documentation translations.