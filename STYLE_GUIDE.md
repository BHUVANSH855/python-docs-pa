# Punjabi (pa-IN) Python Docs Style Guide

This guide defines translation conventions for the Punjabi translation of Python documentation.

## General Principles

* Translate meaning, not individual words.
* Use clear and natural Punjabi (Gurmukhi).
* Maintain consistency across all files.
* Follow terminology defined in `GLOSSARY.md`.
* Preserve technical accuracy at all times.

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
and
or
not
```

### Variable Names

```text
x
y
count
user_name
my_list
self
cls
```

### Function, Class, Module, and Exception Names

Examples:

```text
print
len
range
ValueError
TypeError
Exception
list
dict
tuple
set
os
sys
json
```

These names must remain unchanged.

---

## RST Markup Preservation

Never modify Sphinx or reStructuredText markup.

Examples:

```rst
:func:`print`
:class:`list`
:mod:`os`
:ref:`section`
:meth:`append`
:attr:`name`
:exc:`ValueError`
:term:`iterator`
```

Translate only surrounding explanatory text.

---

## Directives

Preserve directives exactly as written.

Examples:

```rst
.. note::
.. warning::
.. code-block:: python
.. versionadded::
.. versionchanged::
```

Translate the content inside notes and warnings, but never change the directive itself.

---

## Code Blocks

Translate:

* Comments
* User-facing explanatory text

Do not translate:

* Python keywords
* Variable names
* Function names
* Class names
* Module names
* Exception names
* Example code behavior

Example:

```python
# Calculate the square of a number
x = 5
print(x * x)
```

Only the comment may be translated.

---

## URLs

Leave all URLs unchanged.

Examples:

```text
https://docs.python.org/
https://devguide.python.org/
```

---

## Terminology

Always consult `GLOSSARY.md` before introducing new translations.

When a technical term already exists in the glossary, use the glossary version consistently throughout the project.

---

## Consistency Rules

* Use the same translation for the same term everywhere.
* Preserve punctuation when possible.
* Preserve formatting and inline markup.
* Keep examples technically correct after translation.

---

## Machine Translation

Machine translation may be used only as a drafting aid.

Every translated string must be manually reviewed for:

* Accuracy
* Terminology consistency
* Natural Punjabi wording
* Correct markup preservation

Contributors are responsible for the final quality of submitted translations.

---

## Validation Before Commit

Run:

```bash
msgfmt --check tutorial/FILENAME.po
```

Check progress:

```bash
msgfmt --statistics tutorial/FILENAME.po
```

Review untranslated entries:

```bash
msgattrib --untranslated tutorial/FILENAME.po
```

All files should pass validation before submission.

---

## Tone

* Use formal Punjabi.
* Keep explanations clear and educational.
* Prefer consistency over stylistic variation.
* Follow Python documentation writing conventions whenever possible.
