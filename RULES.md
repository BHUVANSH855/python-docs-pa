**# Punjabi Python Documentation Translation Rules**

This document defines the rules contributors must follow before translating

or editing Punjabi (`pa`) Python documentation.

The purpose of these rules is to keep the translation technically accurate,

natural for Punjabi-speaking Python users, consistent across the repository,

and compatible with the official Python documentation tooling.

The primary reference for translation policy is the Python Developer Guide

documentation translation guidance:

https\://devguide.python.org/documentation/translations/translating/

Other official Python documentation translations may be consulted as

references for translation methodology and terminology.

---

**## 1. Core Translation Principles

**### 1.1 Translate meaning, not words**

Translate the meaning of the English documentation into natural Punjabi.

Do not perform word-for-word translation when that produces unnatural,

ambiguous, misleading, or technically incorrect Punjabi.

The final translation should communicate the same technical meaning as the

English source.

**### 1.2 Preserve technical accuracy**

Never simplify, generalize, reinterpret, or alter a technical statement merely

to make the Punjabi sentence easier to write.

Technical behavior described by the English documentation must remain

technically equivalent in Punjabi.

**### 1.3 Punjabi should be natural**

Use Punjabi that a Punjabi-speaking programmer can read naturally.

Avoid:

- machine-translation artifacts

- unnecessarily complicated Punjabi

- unnatural literal translations

- excessive Sanskritized vocabulary

- unnecessary English words when a familiar Punjabi technical form exists

- forced Punjabi translations of technical terms that programmers normally

  know in English

**### 1.4 Do not translate every technical word automatically**

Technical terminology must be decided using context.

For a technical term:

1\. Check existing Punjabi programming/documentation usage.

2\. Check previously approved terminology in this project.

3\. Check established terminology in mature Python documentation translations.

4\. Consider whether Punjabi programmers normally use the English term.

5\. Prefer an established community convention over an invented translation.

6\. A hybrid Punjabi + English form is acceptable when it is natural and

   commonly understood.

7\. English may remain unchanged when it is the clearest or most familiar

   technical form.

8\. Once terminology is approved for this project, record it in the glossary

   and use it consistently.

Do not invent a Punjabi technical term simply because a dictionary provides

a possible translation.

---

**## 2. Technical Terminology Policy

**### 2.1 Use the glossary consistently**

`GLOSSARY.md` is the project's terminology record.

When a term has an approved project translation, use that translation

consistently unless there is a strong technical or contextual reason not to.

Do not introduce competing translations for the same technical concept.

**### 2.2 Glossary entries require review**

A new terminology choice must not be added to `GLOSSARY.md` merely because

one contributor prefers it.

Before adding a new term:

1\. Check existing project translations.

2\. Check Punjabi programming/documentation usage.

3\. Check mature Python translations for translation methodology.

4\. Confirm that the proposed term accurately represents the Python concept.

5\. Prefer a form that will remain understandable to Punjabi programmers.

6\. Use the same term throughout the project after approval.

**### 2.3 Context takes priority**

The same English word may require different Punjabi wording in different

contexts.

For example, an English word may be:

- a Python technical concept

- an ordinary English word

- an identifier

- a class name

- a function name

- part of a Sphinx role

- part of a code example

Do not translate based only on string matching.

**### 2.4 Do not perform blind global replacements**

Never run a repository-wide replacement such as:

```text

method -> Punjabi equivalent

object -> Punjabi equivalent

string -> Punjabi equivalent

```

without checking the context.

A word may occur inside code, identifiers, Sphinx markup, API names, or

other structures where changing it would be incorrect.

---

**## 3. Python Names and Identifiers

The following must remain unchanged unless the English source itself changes:

- Python keywords

- function names

- method names

- class names

- module names

- package names

- exception names

- attribute names

- variable names in code

- argument names in code

- parameter names in code

- constants

- API names

- C API names

- command names

- environment variable names

- file names

- directory names

- protocol names

- PEP numbers

- Python version numbers

Examples:

```text

def

class

return

async

await

__init__

__name__

PyObject

Py_INCREF

StopIteration

Python

CPython

asyncio

```

must not be translated.

---

**## 4. Code Examples

**### 4.1 Preserve executable code**

Do not alter executable Python code unless the English source itself has

changed.

Preserve:

- indentation

- variable names

- function names

- class names

- method names

- operators

- syntax

- imports

- module names

- arguments

- parameters

- strings that are required for program behavior

**### 4.2 Comments may be translated**

Comments inside code examples may be translated when doing so does not change

their meaning.

Example:

```python

\# create a list

```

may have its comment translated, while:

```python

items = []

```

must remain unchanged.

**### 4.3 String literals require context**

Do not automatically translate every string literal.

A string may be:

- explanatory example text

- command output

- expected program output

- an API value

- a protocol value

- an identifier

- data used by the example

Only translate it when the source documentation intends the literal itself

to be translated.

---

**## 5. reStructuredText and Sphinx Markup

Python documentation uses reStructuredText and Sphinx extensively.

Translation must preserve documentation markup.

**### 5.1 Preserve Sphinx roles**

Do not modify the role itself.

Examples:

```text

\:func:`print`

\:class:`list`

\:meth:`str.format`

\:keyword:`while`

\:exc:`ValueError`

\:mod:`asyncio`

\:ref:`some-reference`

\:pep:`703`

```

must retain their role syntax.

**### 5.2 Preserve role targets**

The target of a Sphinx role is normally an internal documentation identifier

and must remain unchanged.

For example:

```text

\:ref:`function`

```

must not become:

```text

\:ref:`ਫੰਕਸ਼ਨ`

```

when `function` is the reference target.

**### 5.3 Explicit display text may be translated**

When a Sphinx role contains separate display text and target, the display

text may be translated while the target remains unchanged.

Example:

```text

\:ref:`Function definitions <function>`

```

may translate the visible label while preserving:

```text

<function>

```

**### 5.4 Preserve directives**

Do not translate directive names or their technical arguments.

Examples:

```text

.. code-block::

.. note::

.. warning::

.. seealso::

.. versionadded::

.. versionchanged::

```

**### 5.5 Preserve links**

Do not change:

- URLs

- URL targets

- anchors

- reference identifiers

Only translate visible link text where appropriate.

---

**## 6. Placeholders and Formatting

Placeholders must remain unchanged.

Examples include:

```text

%s

%d

{value}

{foo}

%(name)s

<feature>

<filename>

```

Do not rename or translate placeholders.

Preserve:

- backticks

- double backticks

- asterisks used for emphasis

- underscores used by reStructuredText

- quotation marks where technically significant

- escaped characters

- newline structure where required

- code formatting

---

**## 7. PO File Rules

### 7.1 English source strings are read-only

**Never intentionally modify the English source strings in `msgid` during
translation, review, cleanup, or terminology work.**

The `msgid` is the upstream English source and must be treated as read-only.

Do not:

- rewrite English wording
- fix English grammar
- change English punctuation
- change English capitalization
- alter the English meaning
- translate the English source
- change source text merely to make the Punjabi translation easier
- make formatting-only edits to `msgid` content as part of translation work

Translation and cleanup work must be performed on `msgstr`.

The only exception is a legitimate upstream source update. If the upstream
Python documentation changes the English source, the PO files may receive the
new `msgid` through the normal source/template synchronization process. That
is not a translation edit.

**A translation-quality change must contain no intentional `msgid` changes.**

### 7.2 `msgstr` is the translation side

All normal Punjabi translation work belongs in `msgstr`.

When reviewing an entry:

1. Read the `msgid` only to understand the source meaning.
2. Decide the correct Punjabi wording.
3. Modify only `msgstr`.
4. Preserve any required source-side markup, identifiers, URLs, placeholders,
   and other technical content.

If the English source itself appears incorrect, do not silently fix it in the
Punjabi PO file. Report or address the upstream source separately.

### 7.3 Preserve PO syntax

Every PO entry must remain valid gettext syntax.

Before committing:

```bash
msgfmt --check -o /dev/null path/to/file.po
```

For repository-wide validation:

```bash
find . -name "*.po" -print0 | xargs -0 -n1 msgfmt --check -o /dev/null
```

### 7.4 Preserve multiline structure

When editing multiline `msgstr` entries:

- preserve valid quoting
- preserve escaped characters
- preserve newline characters
- do not accidentally merge or split content in a way that changes meaning
- ensure the final PO file remains syntactically valid

Do not rewrap or otherwise rewrite `msgid` lines during translation work.

### 7.5 Never leave accidental fuzzy translations

A translation should not be marked fuzzy merely to bypass review.

Uncertain translations should be reviewed and corrected before being treated
as final.

Do not remove a legitimate fuzzy marker without reviewing the translation first.

### 7.6 Do not change unrelated entries

A translation commit should not contain unrelated formatting, source-text,
metadata, or code changes.

In particular, do not use a translation cleanup as an excuse to modify English
`msgid` strings elsewhere in the file.

---

## 8. Translation Quality

Every translated entry should be checked for:

**### Meaning**

Does the Punjabi text communicate the same information?

**### Terminology**

Does it use the project's approved term where one exists?

**### Naturalness**

Would a Punjabi-speaking programmer naturally understand the sentence?

**### Grammar**

Is the Punjabi grammatically and stylistically acceptable?

**### Technical precision**

Could the wording cause a reader to misunderstand Python behavior?

**### Consistency**

Is the same concept translated consistently elsewhere?

**### Markup**

Are all roles, references, links, placeholders, and formatting intact?

---

**## 9. Technical English and Hybrid Forms

English technical terminology is allowed and sometimes preferred.

Use English when:

- the word is commonly used by programmers

- a Punjabi translation is uncommon or confusing

- the word is a proper technical name

- the English form is clearer

- the term is normally used in English in Punjabi programming material

Hybrid wording is also acceptable when it is natural.

For example:

```text

Python interpreter

CPython interpreter

runtime environment

Python API

```

may remain partly English when that is the clearest terminology for the

intended audience.

Do not force an artificial Punjabi translation merely for the sake of having

every word translated.

---

**## 10. Consistency Policy

Once a technical term has been approved:

- use it consistently across the repository

- update the glossary

- use it in new translations

- correct inconsistent completed translations where appropriate

- do not introduce another spelling or translation without review

Consistency applies to:

- terminology

- spelling

- transliteration

- punctuation

- capitalization

- technical names

- recurring documentation phrases

---

**## 11. Terminology Review Procedure

When encountering a technical term without an approved project translation:

**### Step 1**

Check `GLOSSARY.md`.

**### Step 2**

Search completed Punjabi translations in this repository.

**### Step 3**

Check Punjabi programming resources and established usage.

**### Step 4**

Consult mature Python translation projects such as:

- Simplified Chinese

- Traditional Chinese

- Japanese

- Korean

- other established Python documentation translations

These are references for terminology methodology and translation practice,

not sources to copy literally.

**### Step 5**

Check the meaning in the official Python documentation or CPython glossary.

**### Step 6**

Choose the form that is:

- technically accurate

- understandable

- natural in Punjabi

- appropriate for Python programmers

- consistent with existing project terminology

**### Step 7**

Record the approved terminology in `GLOSSARY.md`.

---

**## 12. Do Not Copy Other Languages Literally

Other Python translations are useful references, but their terminology is

language-specific.

A Chinese, Japanese, Korean, Spanish, or French translation must not be

copied mechanically into Punjabi.

Use other translations to understand:

- how technical terms are handled

- when English is retained

- how terminology dictionaries are organized

- how Sphinx markup is preserved

- how translators maintain consistency

The Punjabi translation must follow Punjabi language conventions.

---

**## 13. Review Existing Translations

A previously translated entry is not automatically considered correct.

When reviewing old translations:

- check the English source again

- verify technical meaning

- check terminology against the current glossary

- check consistency with current project rules

- check Sphinx markup

- check code examples

- improve awkward or misleading Punjabi when necessary

However, do not rewrite translations merely because another wording is

personally preferred.

There must be a clear linguistic, technical, or consistency reason for a

change.

---

**## 14. Avoid Machine-Translation Artifacts

Do not submit translations that appear to have been copied directly from an

automatic translation system without human review.

Watch for:

- unnatural word order

- incorrect technical meanings

- inconsistent terminology

- unexplained English/Punjabi switching

- incorrect punctuation

- literal translations of idioms

- incorrect grammatical agreement

- mistranslated code terminology

Machine translation may be used as a drafting aid, but every final translation

must be reviewed by a human.

---

**## 15. Do Not Translate Names

The following should normally remain unchanged:

```text

Python

CPython

PyPI

GitHub

Transifex

Unicode

UTF-8

PEP

PEP 703

Linux

Windows

macOS

POSIX

JSON

XML

HTTP

HTTPS

URL

API

```

Do not translate a proper name merely because a Punjabi transliteration exists.

Transliteration may be used in explanatory prose only when it is appropriate

and does not alter the actual technical name.

---

**## 16. Version and Release Information

Never alter technical version information.

Preserve values such as:

```text

Python 3.15

Python 3.14

3.13

PEP 703

```

exactly when they identify a version, release, or specification.

Do not translate version identifiers.

---

**## 17. Punctuation and Formatting

Punjabi prose should use consistent punctuation.

Be careful with:

- commas

- full stops

- colons

- semicolons

- parentheses

- quotation marks

- hyphens

- dashes

- apostrophes

- code delimiters

Do not introduce formatting changes that are unrelated to translation.

---

**## 18. Source Meaning Has Priority Over Style Preference

When choosing between two valid Punjabi formulations:

1\. Prefer the one that preserves technical meaning most precisely.

2\. Prefer natural Punjabi.

3\. Prefer established project terminology.

4\. Prefer consistency with surrounding documentation.

5\. Do not change wording merely because it sounds more personally preferred.

---

**## 19. Core Switcher Files

The following files are especially important for the Python documentation

translation infrastructure:

```text

bugs.po

tutorial/\*.po

builtins/functions.po

```

These files require particularly careful review because their translation

status is relevant to the documentation language switcher.

Do not sacrifice translation quality merely to increase completion

percentages.

---

**## 20. Validation Before Commit

At minimum, run:

```bash

find . -name "\*.po" -print0 | xargs -0 -n1 msgfmt --check -o /dev/null

```

Then:

```bash

git diff --check

```

Review the actual changes:

```bash

git diff

```

Before committing, confirm:

- no unintended `msgid` changes

- no code changes

- no broken Sphinx markup

- no altered URLs

- no altered placeholders

- no accidental whitespace damage

- no unrelated changes

- no incorrect terminology introduced

Where available, also run the repository's documentation and linting checks.

---

**## 21. Commit Discipline

Keep commits focused.

Good examples:

```text

Update Punjabi documentation translations

Fix Punjabi terminology consistency

Improve Punjabi glossary terminology

Fix Punjabi translation markup

Add Punjabi translation contributor rules

```

Avoid mixing unrelated changes into a translation-quality commit.

---

**## 22. Review Checklist

Before submitting a translation change, confirm:

```text

[ ] Meaning preserved

[ ] Punjabi is natural and readable

[ ] Approved terminology is used

[ ] No unnecessary technical English was introduced

[ ] No required English technical term was incorrectly translated

[ ] Python/API names preserved

[ ] Code preserved

[ ] Sphinx roles preserved

[ ] Sphinx role targets preserved

[ ] URLs preserved

[ ] Placeholders preserved

[ ] PO syntax valid

[ ] No fuzzy translation accidentally introduced

[ ] No unrelated changes

[ ] Translation reviewed by a human

```

---

**## 23. Golden Rule

> Translate the documentation, not the program.

The goal is not to replace every English word.

The goal is to produce accurate, natural, consistent, maintainable Punjabi

documentation for Python users while preserving the technical structure of

the official Python documentation.

When language preference, terminology preference, and technical correctness

conflict, technical correctness and preservation of the source meaning take

priority.

---

**## 24. References

Primary guidance:

- Python Developer Guide — Documentation Translations

  https\://devguide.python.org/documentation/translations/translating/

- Python Documentation

  https\://docs.python.org/

- Python Developer Guide — Documentation Style Guide

  https\://devguide.python.org/documentation/style-guide/

- CPython Glossary

  https\://docs.python.org/3/glossary.html

Useful translation references:

- Python Simplified Chinese Documentation

  https\://github.com/python/python-docs-zh-cn

- Python Traditional Chinese Documentation

  https\://github.com/python/python-docs-zh-tw

- Python Japanese Documentation

  https\://github.com/python/python-docs-ja

These projects should be used as references for translation practice and

terminology methodology, not as sources for literal Punjabi translations.