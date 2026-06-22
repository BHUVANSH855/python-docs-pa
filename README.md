# Translation of the Python Documentation — pa

Punjabi (Gurmukhi) translation of the Python documentation.

This project aims to translate Python's official documentation into Punjabi (Gurmukhi) and make Python learning resources more accessible to Punjabi-speaking developers, students, and educators.

## Status

🎉 All currently tracked translation files are complete and validated.

The repository currently contains fully translated and validated files across:

* Tutorial Documentation
* Core Library Reference
* bugs.po
* glossary.po

All translation files pass GNU gettext validation checks, are tracked in GitHub, and pass repository-wide validation.

Completed major translation milestones:

* `bugs.po`
* `glossary.po`
* `library/functions.po`
* `library/stdtypes.po`
* `library/functools.po`
* `library/exceptions.po`
* Complete Tutorial Documentation Set

**Repository status:** Active development

**Latest milestone:** Language tag standardized to `pa` and translations uploaded to Transifex

### Translation Milestones

| Milestone | Status |
|------------|---------|
| Tutorial Documentation | ✅ Complete |
| bugs.po | ✅ Complete |
| library/functions.po | ✅ Complete |
| library/stdtypes.po | ✅ Complete |
| library/functools.po | ✅ Complete |
| library/exceptions.po | ✅ Complete |
| Repository Validation | ✅ Passing |
| Transifex Upload | ✅ Complete |

## Current Progress

### Completed Tutorial Files

| File | Status | Messages |
|--------|--------|---------:|
| appendix.po | ✅ Complete | 28 |
| appetite.po | ✅ Complete | 17 |
| classes.po | ✅ Complete | 154 |
| controlflow.po | ✅ Complete | 226 |
| datastructures.po | ✅ Complete | 139 |
| errors.po | ✅ Complete | 96 |
| floatingpoint.po | ✅ Complete | 76 |
| inputoutput.po | ✅ Complete | 112 |
| interactive.po | ✅ Complete | 7 |
| interpreter.po | ✅ Complete | 33 |
| introduction.po | ✅ Complete | 120 |
| modules.po | ✅ Complete | 116 |
| stdlib.po | ✅ Complete | 67 |
| stdlib2.po | ✅ Complete | 65 |
| venv.po | ✅ Complete | 42 |
| whatnow.po | ✅ Complete | 18 |

### Completed Root Files

| File | Status | Messages |
|--------|--------|---------:|
| bugs.po | ✅ Complete | 31 |
| glossary.po | ✅ Complete | 30 |

### Completed Library Files

| File | Status | Messages |
|------|--------|---------:|
| functions.po | ✅ Complete | 535 |
| stdtypes.po | ✅ Complete | 1592 |
| functools.po | ✅ Complete | 324 |
| exceptions.po | ✅ Complete | 207 |

### Project Statistics

| Metric | Value |
|----------|------:|
| Tutorial Files Completed | 16 |
| Tutorial Messages Translated | 1,416 |
| Root Files Completed | 2 |
| Root Messages Translated | 61 |
| Library Files Completed | 4 |
| Library Messages Translated | 2,658 |
| Total Messages Translated | 4,135 |

## Validation Status

All completed translation files successfully pass validation.

```bash
msgfmt --check bugs.po
msgfmt --check tutorial/FILENAME.po
msgfmt --check library/FILENAME.po
```

Validation summary:

* ✅ No validation errors
* ✅ No untranslated messages
* ✅ No fuzzy messages
* ✅ Tutorial files validated
* ✅ Library files validated
* ✅ bugs.po validated
* ✅ glossary.po validated
* ✅ Transifex upload complete
* ✅ Repository-wide validation passing
* ✅ GitHub Actions validation passing

## Recent Milestones

* ✅ Completed tutorial documentation set
* ✅ Completed bugs.po
* ✅ Completed library/functions.po
* ✅ Completed library/stdtypes.po
* ✅ Completed library/functools.po
* ✅ Completed library/exceptions.po
* ✅ Standardized language tag to `pa`
* ✅ Uploaded completed translations to Transifex
* ✅ Repository renamed to `python-docs-pa`
* ✅ Repository-wide validation passing
* ✅ All translations committed, validated, and pushed to GitHub

## Infrastructure

* ✅ STYLE_GUIDE.md
* ✅ GLOSSARY.md
* ✅ CONTRIBUTING.md
* ✅ PROJECT_REPORT.md
* ✅ GitHub Actions validation workflow
* ✅ Transifex synchronization workflow
* ✅ Translation terminology consistency review

## Transifex

Punjabi translations are available on the official Python Documentation Transifex project.

Language tag: `pa`

Coordinator: @BHUVANSH855

Current repository translations have been uploaded to Transifex.

## Next Phase

Current priorities:

1. Review repository structure against docsbuild-scripts requirements
2. Open Python Devguide translation listing PR
3. Configure automated Transifex synchronization
4. Expand translation coverage into:
   * Reference Documentation
   * Using Python Documentation
   * What's New Documentation
5. Grow the Punjabi translation community

## Goals

Project goals are aligned with the Python Documentation Translation initiative and focus on expanding Punjabi-language access to Python learning resources while maintaining translation quality and terminology consistency.

* Translate Python documentation into Punjabi (Gurmukhi)
* Maintain terminology consistency through a shared glossary
* Follow Python documentation translation guidelines
* Ensure translation quality through automated validation
* Build a contributor community around Punjabi translations
* Contribute to the Python documentation translation ecosystem

## Repository Structure

```text
python-docs-pa/
├── .gitignore
├── bugs.po
├── glossary.po
├── CONTRIBUTING.md
├── GLOSSARY.md
├── PROJECT_REPORT.md
├── README.md
├── STYLE_GUIDE.md
│
├── .github/
│   └── workflows/
│       ├── validate.yml
│       └── transifex-pull.yml
│
├── tutorial/
│   ├── appendix.po
│   ├── appetite.po
│   ├── classes.po
│   ├── controlflow.po
│   ├── datastructures.po
│   ├── errors.po
│   ├── floatingpoint.po
│   ├── index.po
│   ├── inputoutput.po
│   ├── interactive.po
│   ├── interpreter.po
│   ├── introduction.po
│   ├── modules.po
│   ├── stdlib.po
│   ├── stdlib2.po
│   ├── venv.po
│   └── whatnow.po
│
├── library/
│   ├── exceptions.po
│   ├── functions.po
│   ├── functools.po
│   └── stdtypes.po
│
├── reference/
├── using/
└── whatsnew/
```

## Translation Workflow

1. Translate `.po` files.
2. Validate translations:

```bash
msgfmt --check FILE.po
```

3. Review terminology against `GLOSSARY.md`.
4. Follow rules in `STYLE_GUIDE.md`.
5. Ensure RST roles, directives, and code blocks remain unchanged.
6. Commit and push changes.
7. Verify GitHub Actions passes successfully.

## References

Python Documentation Translation Guide:

https://devguide.python.org/documentation/translations/

Python Documentation Project:

https://docs.python.org/

Python Documentation Translation Platform:

https://app.transifex.com/python-doc/python-newest/

## License

Documentation translations are contributed under the CC0 license.
