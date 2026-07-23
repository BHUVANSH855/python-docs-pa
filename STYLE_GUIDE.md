# Punjabi (pa) Python Docs Style Guide

This guide defines translation conventions for the Punjabi (`pa`) translation of the Python documentation.

It complements `README.md`, `CONTRIBUTING.md`, and `GLOSSARY.md` by describing the writing style, terminology, formatting rules, and validation practices contributors should follow when translating Python documentation.

All contributors should follow these guidelines to ensure consistency, technical accuracy, and long-term maintainability across the project.

---

## Contents

- [Project Status](#project-status)
- [General Principles](#general-principles)
- [Translation Philosophy](#translation-philosophy)
- [Never Translate](#never-translate)
- [Variable Names](#variable-names)
- [PO File Rules](#po-file-rules)
- [Placeholder Preservation](#placeholder-preservation)
- [RST Markup Preservation](#rst-markup-preservation)
- [Inline Markup Preservation](#inline-markup-preservation)
- [Directives](#directives)
- [Code Blocks](#code-blocks)
- [Interactive Python Sessions](#interactive-python-sessions)
- [URLs](#urls)
- [Version Information](#version-information)
- [Technical Terms](#technical-terms)
- [Terminology Consistency](#terminology-consistency)
- [Batch Translation Workflow](#batch-translation-workflow)
- [Machine Translation Policy](#machine-translation-policy)
- [Translation Quality Checklist](#translation-quality-checklist)
- [Validation Commands](#validation-commands)
- [Repository-Wide Validation](#repository-wide-validation)
- [Transifex Synchronization](#transifex-synchronization)
- [Commit Message Conventions](#commit-message-conventions)
- [Contributor Expectations](#contributor-expectations)
- [Tone and Writing Style](#tone-and-writing-style)
- [Translation Review](#translation-review)
- [Final Rule](#final-rule)

---

# Project Status

The Punjabi (`pa`) translation project is actively maintained as part of the official Python Documentation Translation initiative.

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
| Tutorial Files | 17 |
| Using Python Files | 9 |
| Completed Core Library Files | 5 |
| Completed HOWTO Files | 2 |
| Root Translation Files | 2 |

Contributors should review previously completed translations before introducing new terminology or translation patterns.

---

# General Principles

The following principles apply to every translation in this repository, regardless of the document or subject area.

* Translate meaning, not individual words.
* Use natural and clear Punjabi (Gurmukhi).
* Preserve technical accuracy.
* Prefer consistency over stylistic variation.
* Follow terminology defined in `GLOSSARY.md`.
* Reuse existing translations whenever possible.
* Match the tone of official Python documentation.

---

# Translation Philosophy

The goal is not literal translation.

The goal is to produce documentation that feels natural to Punjabi-speaking developers while remaining technically identical to the English original.

Good translation:

```text
Clear
Accurate
Consistent
Natural
```

Poor translation:

```text
Word-for-word
Ambiguous
Inconsistent
Artificial sounding
```

---

# Never Translate

## Python Keywords

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
and
or
not
global
nonlocal
async
await
match
case
```

---

## Built-in Names

```text
print
len
range
list
dict
tuple
set
frozenset
bytes
bytearray
str
int
float
complex
bool
object
type
property
classmethod
staticmethod
```

---

## Exception Names

```text
Exception
ValueError
TypeError
KeyError
IndexError
ImportError
RuntimeError
AttributeError
StopIteration
```

---

## Standard Library Names

```text
os
sys
json
pathlib
re
typing
collections
itertools
asyncio
```

These identifiers must remain unchanged.

---

# Variable Names

Never translate variable names.

Examples:

```python
x
y
count
index
user_name
my_list
self
cls
```

Correct:

```python
count = 5
```

Incorrect:

```python
ਗਿਣਤੀ = 5
```

---

# PO File Rules

Never modify:

```text
msgid
#: source references
#, flags
```

Translate only:

```text
msgstr
```

---

# Placeholder Preservation

Placeholders must remain exactly unchanged.

Examples:

```text
%s
%d
%i
%r
%f
%s%.*f
```

```text
{}
{0}
{name}
{value}
```

```text
%(name)s
%(count)d
```

Correct:

```text
"%s ਆਈਟਮ ਮਿਲੇ"
```

Incorrect:

```text
"%d ਆਈਟਮ ਮਿਲੇ"
```

unless the original uses `%d`.

---

# RST Markup Preservation

Never modify reStructuredText roles.

Examples:

```rst
:func:`print`
:class:`list`
:class:`dict`
:mod:`os`
:meth:`append`
:attr:`name`
:exc:`ValueError`
:term:`iterator`
:ref:`section`
```

Translate only surrounding text.

Correct:

```rst
ਇਹ :func:`print` ਫੰਕਸ਼ਨ ਦੀ ਵਰਤੋਂ ਕਰਦਾ ਹੈ।
```

Incorrect:

```rst
ਇਹ :func:`ਛਾਪੋ` ਫੰਕਸ਼ਨ ਦੀ ਵਰਤੋਂ ਕਰਦਾ ਹੈ।
```

---

# Inline Markup Preservation

Keep inline markup unchanged.

Examples:

```rst
*italic*
**bold**
``code``
```

Do not modify formatting syntax.

---

# Directives

Never modify Sphinx directives.

Examples:

```rst
.. note::
.. warning::
.. important::
.. tip::
.. versionadded::
.. versionchanged::
.. deprecated::
.. code-block:: python
```

Translate the directive content only.

---

# Code Blocks

Translate:

* Comments
* Explanatory text

Do not translate:

* Python code
* Keywords
* Identifiers
* Module names
* Function names
* Class names
* Exception names

Example:

```python
# Calculate the square of a number
x = 5
print(x * x)
```

Only the comment may be translated.

---

# Interactive Python Sessions

Examples:

```python
>>> x = 5
>>> print(x)
5
```

Do not translate:

* Code
* Output
* Tracebacks
* Exception names

Translate only surrounding explanations.

---

# URLs

Never translate URLs.

Examples:

```text
https://docs.python.org/
https://devguide.python.org/
https://github.com/python/cpython
```

---

# Version Information

Never modify version numbers.

Examples:

```text
Python 3.13
Python 3.14
Changed in version 3.12
Deprecated since version 3.11
```

Translate surrounding text only.

---

# Technical Terms

Some technical terms are widely recognized in English within the Python ecosystem and should normally remain untranslated unless the project glossary specifies an approved Punjabi equivalent.

Examples:

```text
Python
API
Unicode
JSON
XML
HTML
HTTP
URL
ASCII
UTF-8
```

Use glossary-approved Punjabi translations where available.

---

# Terminology Consistency

Always consult:

```text
GLOSSARY.md
```

before introducing new terminology.

If a term already exists in the glossary:

* Use the glossary translation.
* Do not create alternatives.
* Do not switch wording between files.

Consistency is more important than personal preference.

---

# Batch Translation Workflow

For large files, translations should be performed in reviewable batches.

Recommended format:

```text
Replace this block:

msgid "example"
msgstr ""

With:

msgid "example"
msgstr "ਉਦਾਹਰਨ"
```

For multiple consecutive entries:

```text
Replace these consecutive blocks:
...
```

This workflow was successfully used for:

```text
library/functions.po
library/stdtypes.po
library/functools.po
library/exceptions.po
```

and is recommended for future large files.

---

# Machine Translation Policy

Machine translation may be used only as a drafting aid.

Every translation must be manually reviewed.

Contributors remain responsible for:

* Accuracy
* Technical correctness
* Terminology consistency
* Markup preservation
* Natural Punjabi wording

No untranslated machine output should be committed.

---

# Translation Quality Checklist

Before committing:

* Verify all intended strings are translated.
* Verify placeholders remain unchanged.
* Verify markup remains unchanged.
* Verify code examples remain executable.
* Verify glossary terminology is followed.
* Verify formatting matches the source.
* Verify the documentation builds successfully.
* Verify `sphinx-lint` reports no issues.
* Verify the translation reads naturally in Punjabi.
* Complete a manual review.

---

# Validation Commands

Validate a file:

```bash
msgfmt --check FILE.po
```

Show statistics:

```bash
msgfmt --statistics FILE.po
```

Show untranslated entries:

```bash
msgattrib --untranslated FILE.po
```

Show translated entries:

```bash
msgattrib --translated FILE.po
```

---

# Repository-Wide Validation

Validate translation files:

```bash
msgfmt --check FILE.po
```

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

A completed translation should:

- Pass GNU gettext validation.
- Preserve all reStructuredText markup.
- Produce no `sphinx-lint` errors.
- Build successfully with CPython's HTML documentation builder.
- Pass the nitpicky (`-n`) documentation build.

---

# Transifex Synchronization

Translations may be maintained through the official Python Documentation
Transifex project.

Before uploading translations:

* Validate all files with msgfmt
* Ensure glossary terminology is consistent
* Verify RST markup remains unchanged
* Review all machine-assisted translations manually

Only validated translations should be uploaded.

---

# Commit Message Conventions

Commit messages should be concise, descriptive, and focused on a single logical change whenever possible.

Use descriptive commit messages.

Examples:

```text
Translate tutorial/classes.po to Punjabi
Translate tutorial/floatingpoint.po to Punjabi
Translate tutorial/venv.po to Punjabi
Translate library/functions.po to Punjabi
Translate library/stdtypes.po to Punjabi
Translate library/functools.po to Punjabi
Translate library/exceptions.po to Punjabi
Translate glossary.po to Punjabi
Update glossary terminology
Update README statistics
Update project documentation
```

---

# Contributor Expectations

Before starting a new file:

1. Review `GLOSSARY.md`
2. Review this Style Guide
3. Review completed translations
4. Validate frequently
5. Commit in logical batches
6. Keep terminology consistent

---

# Tone and Writing Style

Documentation should be:

* Formal
* Educational
* Clear
* Consistent
* Professional

Avoid:

* Slang
* Regional dialect variations
* Excessively literal translations
* Unnecessary English/Punjabi mixing

When in doubt:

```text
Clarity > Literal Translation
Consistency > Personal Preference
Accuracy > Style
```

---

# Translation Review

Every completed translation should be reviewed before submission.

Review each completed translation for:

- Technical accuracy.
- Natural and idiomatic Punjabi wording.
- Consistent terminology.
- Correct grammar and spelling.
- Preservation of placeholders.
- Preservation of reStructuredText markup.
- Formatting consistency.
- Successful validation with the project's tooling.

---

# References

Useful resources for contributors:

- **Python Developer Guide – Documentation Translations**  
  <https://devguide.python.org/documentation/translations/>

- **Python Documentation**  
  <https://docs.python.org/>

- **Python Documentation Style Guide**  
  <https://devguide.python.org/documentation/style-guide/>

- **Python Documentation on Transifex**  
  <https://app.transifex.com/python-doc/python-newest/>

- **reStructuredText Primer (Sphinx)**  
  <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>

---

# Final Rule

Every translation should satisfy three requirements:

```text
Technically accurate
Consistent with the project glossary
Natural and readable for Punjabi users
```

If any of these requirements are not met, revise the translation before committing.
