# Translation of the Python Documentation — pa

[![Python Version](https://img.shields.io/badge/Python-3.15-blue.svg)](https://www.python.org/)
[![Language](https://img.shields.io/badge/Language-Punjabi%20(pa)-green.svg)](https://devguide.python.org/documentation/translations/)
[![License](https://img.shields.io/badge/License-CC0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

Punjabi (Gurmukhi) translation of the Python documentation.

This project aims to translate Python's official documentation into Punjabi (Gurmukhi) and make Python learning resources more accessible to Punjabi-speaking developers, students, and educators.

## Contents

- [Status](#status)
- [Current Progress](#current-progress)
- [Validation Status](#validation-status)
- [Recent Milestones](#recent-milestones)
- [Infrastructure](#infrastructure)
- [Transifex](#transifex)
- [Next Steps](#next-steps)
- [Goals](#goals)
- [Repository Structure](#repository-structure)
- [Translation Workflow](#translation-workflow)
- [References](#references)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## Status

🎉 **Officially recognized** — Punjabi (`pa`) is now listed in the **Python Developer Guide Translation Coordinators** following the merge of **PR #1843**.

This repository follows the official Python Documentation Translation workflow and is synchronized with the official Python Documentation Transifex project.

| Property | Value |
|----------|-------|
| Repository Status | Active Development |
| Current Branch | `3.15` |
| Language Tag | `pa` |

### Translation Progress

| Section | Status | Strings |
|---------|--------|--------:|
| Tutorial (17/17 files) | ✅ Complete | 1,327 |
| Using Python (9/9 files) | ✅ Complete | 1,631 |
| `library/stdtypes.po` | ✅ Complete | 1,607 |
| `library/functions.po` | ✅ Complete | 536 |
| `library/exceptions.po` | ✅ Complete | 207 |
| `library/functools.po` | ✅ Complete | 128 |
| `library/string.po` | ✅ Complete | 31 |
| `howto/regex.po` | ✅ Complete | 335 |
| `howto/sorting.po` | ✅ Complete | 90 |
| `glossary.po` | ✅ Complete | 499 |
| `bugs.po` | ✅ Complete | 31 |
| **Verified Translation Total** | | **7,668** |

### Infrastructure Status

| Component | Status |
|-----------|--------|
| Python Developer Guide Listing | ✅ PR #1843 Merged |
| Transifex Team | ✅ Active |
| Transifex Pull Workflow | ✅ Running Daily |
| GitHub Actions Validation | ✅ Passing |
| GNU gettext (`msgfmt`) Validation | ✅ Passing |
| `sphinx-lint` | ✅ No Problems Found |
| HTML Documentation Build | ✅ Passing |
| Nitpicky (`-n`) Build | ✅ Passing |

## Current Progress

The Punjabi translation project continues to expand through the official Python Documentation Translation workflow.

### Completed Translation Areas

| Area | Status |
|------|--------|
| Tutorial Documentation (17/17 files) | ✅ Complete |
| Using Python Documentation (9/9 files) | ✅ Complete |
| Core Library Translation Set | ✅ Complete |
| `bugs.po` | ✅ Complete |
| `glossary.po` | ✅ Complete |
| `howto/regex.po` | ✅ Complete |
| `howto/sorting.po` | ✅ Complete |

### Translation Statistics

| Metric | Value |
|--------|------:|
| Verified Translated Strings | **7,668** |
| Tutorial Files | 17 |
| Using Python Files | 9 |
| Completed Core Library Files | 5 |
| Completed HOWTO Files | 2 |
| Root Translation Files | 2 |

Translation work is ongoing, with additional Library, HOWTO, FAQ, Reference, C API, and What's New documentation being translated through the official Python Documentation Transifex project.

## Validation Status

All completed translations are validated using the same workflow adopted by the Python Documentation Translation community before being merged into the repository.

### Validation Pipeline

```text
Translate
      ↓
Transifex
      ↓
GitHub Actions Sync
      ↓
GNU gettext Validation (`msgfmt --check`)
      ↓
sphinx-lint
      ↓
CPython HTML Build
      ↓
Nitpicky (`-n`) Documentation Build
```

### Validation Commands

```bash
msgfmt --check FILE.po
sphinx-lint .
python -m sphinx -b html -D language=pa Doc build/html-pa
python -m sphinx -b html -n -W Doc build/html-pa
```

### Validation Summary

- ✅ GNU gettext (`msgfmt`) validation passing
- ✅ No validation errors
- ✅ GitHub Actions validation passing
- ✅ `sphinx-lint` — No problems found
- ✅ CPython HTML documentation build passing
- ✅ Nitpicky (`-n`) documentation build passing
- ✅ Repository-wide validation passing

## Recent Milestones

- ✅ Punjabi (`pa`) officially listed in the Python Developer Guide Translation Coordinators (PR #1843 merged)
- ✅ Repository renamed to `python-docs-pa`
- ✅ Language tag standardized to `pa`
- ✅ Migration to the `3.15` translation branch
- ✅ Tutorial documentation completed (17/17 files)
- ✅ Using Python documentation completed (9/9 files)
- ✅ Core library translation set expanded
- ✅ HOWTO translations (`regex.po` and `sorting.po`) completed
- ✅ 7,668 verified translated strings
- ✅ Daily Transifex synchronization workflow operational
- ✅ GitHub Actions validation passing
- ✅ `sphinx-lint` validation passing
- ✅ CPython HTML and nitpicky documentation builds passing

## Infrastructure

The project includes documentation, automation, and validation resources to ensure consistent, high-quality translations.

| Component | Purpose |
|-----------|---------|
| `STYLE_GUIDE.md` | Translation conventions and style guidelines |
| `GLOSSARY.md` | Standardized Python terminology (English → Punjabi) |
| `CONTRIBUTING.md` | Contributor onboarding and workflow |
| `PROJECT_REPORT.md` | Project history and major milestones |
| GitHub Actions | Automated validation and Transifex synchronization |
| Transifex | Collaborative translation platform |
| GNU gettext (`msgfmt`) | Translation validation |
| `sphinx-lint` | Documentation quality checks |
| CPython HTML Build | Verifies successful documentation builds |
| Nitpicky (`-n`) Build | Detects broken references and documentation issues |

## Transifex

The Punjabi (`pa`) translation is maintained through the official Python Documentation project on Transifex.

### Project Information

| Item | Value |
|------|-------|
| Platform | Python Documentation on Transifex |
| Language | Punjabi (`pa`) |
| Branch | `3.15` |
| Repository | `python-docs-pa` |
| Coordinator | @BHUVANSH855 |

Translations are contributed through Transifex and synchronized to this repository using the automated GitHub Actions workflow.

## Next Steps

Current priorities:

1. Expand translation coverage across additional Library modules (such as `re`, `os`, `pathlib`, and `datetime`).
2. Continue translating HOWTO, FAQ, Reference, C API, and What's New documentation.
3. Continue community review and terminology consistency checks through Transifex.
4. Prepare the project for inclusion in Python's `docsbuild-scripts`.
5. Continue growing the Punjabi translation community and onboarding new contributors.

## Goals

This project supports the Python Documentation Translation initiative by making the official Python documentation accessible to Punjabi speakers while maintaining the same quality standards as the upstream project.

The primary goals are to:

- Translate the official Python documentation into Punjabi (Gurmukhi).
- Maintain consistent terminology through a shared glossary.
- Follow the Python documentation translation guidelines and style conventions.
- Ensure translation quality through automated validation and documentation builds.
- Encourage community contributions and collaborative review.
- Keep translations synchronized with the upstream Python documentation.

## Repository Structure

```text
python-docs-pa/
├── .github/              # GitHub Actions workflows
├── tutorial/             # Tutorial documentation
├── using/                # Using Python documentation
├── library/              # Standard library reference
├── howto/                # HOWTO guides
├── faq/                  # Frequently asked questions
├── reference/            # Language reference
├── c-api/                # Python/C API documentation
├── extending/            # Extending and embedding Python
├── installing/           # Installation documentation
├── distributing/         # Distribution guides
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

## Translation Workflow

The project follows the standard Python Documentation Translation workflow.

```text
Translate in Transifex
          ↓
Review terminology (GLOSSARY.md)
          ↓
Follow translation conventions (STYLE_GUIDE.md)
          ↓
Automated synchronization to GitHub
          ↓
GitHub Actions validation
          ↓
GNU gettext validation (`msgfmt`)
          ↓
sphinx-lint
          ↓
CPython HTML & Nitpicky builds
```

### Contributor Checklist

1. Translate or review `.po` files in Transifex.
2. Follow the terminology defined in `GLOSSARY.md`.
3. Follow the conventions described in `STYLE_GUIDE.md`.
4. Preserve all reStructuredText roles, directives, code blocks, and markup.
5. Validate translations locally when possible.
6. Ensure GitHub Actions complete successfully after synchronization.

## References

The following resources are used throughout this project:

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

## Acknowledgements

This project follows the official Python Documentation Translation initiative.

Special thanks to the Python Documentation community, translation coordinators, reviewers, and contributors whose guidance and infrastructure make community-driven documentation translations possible.

## License

This repository follows the licensing model of the official Python Documentation Translation project.

Documentation translations are contributed under the CC0 1.0 Universal license. See the Python Documentation Translation project for additional licensing information.
