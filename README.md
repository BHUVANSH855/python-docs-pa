# Translation of the Python Documentation — pa-IN

Punjabi (India) translation of the Python documentation.

This project aims to translate Python's official documentation into Punjabi (Gurmukhi) and make Python learning resources more accessible to Punjabi-speaking developers, students, and educators.

## Status

🚧 Work in Progress

Current focus: completing `tutorial/classes.po` and preparing completed translations for Transifex upload.

## Current Progress

### Completed Tutorial Files

| File              | Status     | Messages |
| ----------------- | ---------- | -------- |
| introduction.po   | ✅ Complete | 120      |
| interpreter.po    | ✅ Complete | 33       |
| appetite.po       | ✅ Complete | 17       |
| controlflow.po    | ✅ Complete | 226      |
| datastructures.po | ✅ Complete | 139      |
| inputoutput.po    | ✅ Complete | 112      |
| modules.po        | ✅ Complete | 116      |
| errors.po         | ✅ Complete | 96       |

**Completed tutorial strings:** 859

### In Progress

| File       | Progress         |
| ---------- | ---------------- |
| classes.po | 49 / 154 (31.8%) |

### Infrastructure

* ✅ STYLE_GUIDE.md
* ✅ GLOSSARY.md
* ✅ CONTRIBUTING.md
* ✅ GitHub Actions validation workflow
* ✅ Repository structure aligned with Python documentation translation recommendations

## Goals

* Translate Python documentation into Punjabi (Gurmukhi)
* Maintain terminology consistency through a shared glossary
* Follow Python documentation translation guidelines
* Ensure translation quality through automated validation
* Build a contributor community around Punjabi translations
* Contribute to the Python documentation translation ecosystem

## Repository Structure

```text
python-docs-pa-in/
├── README.md
├── CONTRIBUTING.md
├── GLOSSARY.md
├── STYLE_GUIDE.md
├── .github/
│   └── workflows/
│       └── validate.yml
├── tutorial/
│   ├── appetite.po
│   ├── classes.po
│   ├── controlflow.po
│   ├── datastructures.po
│   ├── errors.po
│   ├── inputoutput.po
│   ├── interpreter.po
│   ├── introduction.po
│   └── modules.po
├── library/
├── reference/
├── using/
└── whatsnew/
```

## Translation Workflow

1. Translate `.po` files.
2. Validate translations:

```bash
msgfmt --check tutorial/FILENAME.po
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

## License

Documentation translations are contributed under the CC0 license.
