# Contributing to Python Docs Punjabi (pa)

Thank you for contributing to the Punjabi (Gurmukhi) translation of the Python documentation.

This project follows the Python Documentation Translation Guidelines and aims to provide high-quality Punjabi (Gurmukhi) translations for Python learners, educators, and developers.

## Current Project Status

### Completed

✅ Complete Tutorial documentation translated and validated (17 files)

✅ `bugs.po` fully translated and validated

✅ `glossary.po` fully translated and validated

✅ `library/functions.po` fully translated and validated

✅ `library/stdtypes.po` fully translated and validated

✅ `library/functools.po` fully translated and validated

✅ `library/exceptions.po` fully translated and validated

✅ Language tag standardized to `pa`

✅ All completed translations uploaded to Transifex

✅ 4,155 documentation messages translated

### Current Focus

Current priorities:

* Automated Transifex synchronization
* Python documentation translation coordination
* Python Devguide translation listing
* Repository structure verification
* Reference documentation
* Using Python documentation
* What's New documentation

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

## Workflow

1. Fork the repository (external contributors).
2. Create a feature branch.
3. Select an untranslated `.po` file.
4. Translate or review entries.
5. Validate the file.
6. Commit your changes.
7. Push to your fork.
8. Open a Pull Request.

## Creating a New Translation File

Generate a new `.po` file from the latest CPython gettext template:

```bash
msginit \
  --locale=pa \
  --input=PATH_TO_TEMPLATE.pot \
  --output-file=PATH_TO_OUTPUT.po
```

Example:

```bash
msginit \
  --locale=pa \
  --input=library/functions.pot \
  --output-file=library/functions.po
```

## Validation

### Check for syntax errors

```bash
msgfmt --check FILE.po
```

### View translation statistics

```bash
msgfmt --statistics FILE.po
```

### Show untranslated entries

```bash
msgattrib --untranslated FILE.po
```

### Show translated entries

```bash
msgattrib --translated FILE.po
```

## Translation Rules

### Never Translate

#### Python Keywords

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

#### Python Identifiers

* Function names
* Class names
* Module names
* Exception names
* Variable names

Examples:

```text
print
len
range
ValueError
TypeError
list
dict
tuple
set
os
sys
json
```

#### Documentation Markup

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

#### Other Items

* URLs
* Code syntax
* File names
* Package names
* Python version numbers

### Translate

* Titles and headings
* Explanatory text
* Notes and warnings
* Comments inside examples
* User-facing descriptions
* Table content
* Documentation narratives

## Quality Checklist

Before submitting a Pull Request:

* [ ] All intended entries translated
* [ ] msgfmt validation passes
* [ ] No broken RST markup
* [ ] No modified code examples
* [ ] Terminology follows GLOSSARY.md
* [ ] Style follows STYLE_GUIDE.md
* [ ] Translation reviewed for natural Punjabi wording
* [ ] GitHub Actions validation passes

## Commit Message Examples

```text
Translate library/functions.po to Punjabi

Translate reference/datamodel.po to Punjabi

Update glossary terminology

Improve translation consistency

Fix validation issues in library modules
```

## Translation Standards

Contributors should:

* Prefer natural Punjabi over literal word-for-word translation.
* Preserve technical accuracy.
* Maintain terminology consistency.
* Keep formatting identical to the source.
* Preserve all Sphinx and reStructuredText markup.
* Follow existing translation patterns established in completed project files (`bugs.po`, `glossary.po`, `tutorial/`, `library/functions.po`, `library/stdtypes.po`, `library/functools.po`, and `library/exceptions.po`).

## Getting Help

Before introducing new terminology, review:

* GLOSSARY.md
* STYLE_GUIDE.md

For translation discussions, suggestions, and coordination, use GitHub Issues and Pull Requests.

## License

Documentation translations are contributed under the CC0 license, consistent with Python Documentation Translation project guidelines.
