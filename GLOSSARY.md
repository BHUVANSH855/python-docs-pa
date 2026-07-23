# Punjabi (pa) Python Docs Glossary

This glossary defines the preferred Punjabi terminology for translating the official Python documentation into Punjabi (`pa`).

It complements `README.md`, `CONTRIBUTING.md`, and `STYLE_GUIDE.md` by providing standardized translations for technical terms used throughout the project.

All contributors should use the terminology defined in this glossary to ensure consistency, technical accuracy, and long-term maintainability across all translated documentation.

---

## Contents

- [Project Status](#project-status)
- [How to Use This Glossary](#how-to-use-this-glossary)
- [Core Python Terms](#core-python-terms)
- [Data Types](#data-types)
- [Mutability](#mutability)
- [Operators and Operations](#operators-and-operations)
- [Collections and Iteration](#collections-and-iteration)
- [Exceptions and Errors](#exceptions-and-errors)
- [Modules and Libraries](#modules-and-libraries)
- [String and Formatting Terms](#string-and-formatting-terms)
- [Numeric Terms](#numeric-terms)
- [Standard Library Terms](#standard-library-terms)
- [Documentation Terms](#documentation-terms)
- [Documentation Workflow Terms](#documentation-workflow-terms)
- [Terms Commonly Left Untranslated](#terms-commonly-left-untranslated)
- [Common Python Keywords](#common-python-keywords)
- [Language Tag](#language-tag)
- [Consistency Rules](#consistency-rules)
- [Glossary Maintenance](#glossary-maintenance)
- [References](#references)
- [Final Notes](#final-notes)

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

The terminology defined in this glossary reflects the vocabulary established throughout the completed translations and should be treated as the project's preferred terminology for all future documentation.

---

# How to Use This Glossary

This glossary establishes the standard terminology for the Punjabi (`pa`) translation of the Python documentation.

When translating documentation:

- Always use glossary-approved terminology whenever a term already exists.
- Do not introduce alternative translations for established technical terms.
- Reuse terminology from previously completed translations whenever possible.
- Follow the writing conventions described in `STYLE_GUIDE.md`.
- Preserve technical accuracy while producing natural and readable Punjabi.

If a required technical term is not yet included in this glossary:

1. Check previously completed translation files for an established translation.
2. Use consistent terminology throughout the document.
3. Add the new term to this glossary only after it has been reviewed and adopted as the project's preferred translation.

---

# Core Python Terms

| English | Preferred Punjabi |
|---------|-------------------|
| function | ਫੰਕਸ਼ਨ |
| built-in function | ਬਿਲਟ-ਇਨ ਫੰਕਸ਼ਨ |
| method | ਵਿਧੀ |
| class | ਕਲਾਸ |
| object | ਵਸਤੂ |
| instance | ਇੰਸਟੈਂਸ |
| attribute | ਐਟ੍ਰਿਬਿਊਟ |
| variable | ਵੇਰੀਏਬਲ |
| parameter | ਪੈਰਾਮੀਟਰ |
| argument | ਆਰਗੂਮੈਂਟ |
| positional argument | ਸਥਿਤੀਗਤ ਆਰਗੂਮੈਂਟ |
| keyword argument | ਕੀਵਰਡ ਆਰਗੂਮੈਂਟ |
| statement | ਕਥਨ |
| expression | ਅਭਿਵ੍ਯੰਜਨਾ |
| namespace | ਨੇਮਸਪੇਸ |
| scope | ਸਕੋਪ |
| inheritance | ਵਿਰਾਸਤ |
| multiple inheritance | ਬਹੁ-ਵਿਰਾਸਤ |
| iterator | ਇਟਰੇਟਰ |
| iteration | ਇਟਰੇਸ਼ਨ |
| iterable | ਇਟਰੇਬਲ |
| generator | ਜਨਰੇਟਰ |
| decorator | ਡੇਕੋਰੇਟਰ |
| callable | ਕਾਲੇਬਲ |
| descriptor | ਡਿਸਕ੍ਰਿਪਟਰ |
| property | ਪ੍ਰਾਪਰਟੀ |
| protocol | ਪ੍ਰੋਟੋਕੋਲ |
| context manager | ਕਾਨਟੈਕਸਟ ਮੈਨੇਜਰ |
| context management | ਕਾਨਟੈਕਸਟ ਪ੍ਰਬੰਧਨ |
| context management protocol | ਕਾਨਟੈਕਸਟ ਪ੍ਰਬੰਧਨ ਪ੍ਰੋਟੋਕੋਲ |
| coroutine | ਕੋਰੂਟੀਨ |
| asynchronous | ਅਸਿੰਕ੍ਰੋਨਸ |
| synchronous | ਸਿੰਕ੍ਰੋਨਸ |

---

# Data Types

| English | Preferred Punjabi |
|---------|-------------------|
| type | ਕਿਸਮ |
| numeric | ਸੰਖਿਆਤਮਕ |
| integer | ਪੂਰਨ ਅੰਕ |
| floating-point | ਫਲੋਟਿੰਗ-ਪੌਇੰਟ |
| complex number | ਕੰਪਲੈਕਸ ਨੰਬਰ |
| boolean | ਬੁਲੀਅਨ |
| string | ਸਤਰ |
| text sequence | ਪਾਠ ਕ੍ਰਮ |
| list | ਸੂਚੀ |
| tuple | ਟਪਲ |
| set | ਸੈੱਟ |
| dictionary | ਡਿਕਸ਼ਨਰੀ |
| mapping | ਮੈਪਿੰਗ |
| range | ਰੇਂਜ |
| bytes | ਬਾਈਟਸ |
| bytearray | ਬਾਈਟਐਰੇ |
| memoryview | ਮੈਮੋਰੀਵਿਊ |
| array | ਐਰੇ |
| sequence | ਕ੍ਰਮ |
| mutable sequence | ਪਰਿਵਰਤਨਯੋਗ ਕ੍ਰਮ |
| immutable sequence | ਅਪਰਿਵਰਤਨਯੋਗ ਕ੍ਰਮ |
| type hint | ਟਾਈਪ ਹਿੰਟ |
| type annotation | ਟਾਈਪ ਐਨੋਟੇਸ਼ਨ |
| alias | ਉਪਨਾਮ |
| enumeration | ਐਨਿਊਮੇਰੇਸ਼ਨ |
| dataclass | ਡਾਟਾਕਲਾਸ |

---

# Mutability

| English | Preferred Punjabi |
|---------|-------------------|
| mutable | ਪਰਿਵਰਤਨਯੋਗ |
| immutable | ਅਪਰਿਵਰਤਨਯੋਗ |
| hash | ਹੈਸ਼ |
| hashing | ਹੈਸ਼ਿੰਗ |

---

# Operators and Operations

| English | Preferred Punjabi |
|---------|-------------------|
| operation | ਕਾਰਵਾਈ |
| arithmetic | ਅੰਕਗਣਿਤ |
| comparison | ਤੁਲਨਾ |
| concatenation | ਜੋੜ |
| repetition | ਦੁਹਰਾਵਾ |
| assignment | ਅਸਾਈਨਮੈਂਟ |
| subscript | ਸਬਸਕ੍ਰਿਪਟ |
| slice | ਸਲਾਈਸ |
| bitwise | ਬਿੱਟਵਾਈਜ਼ |
| masking | ਮਾਸਕਿੰਗ |
| shifting | ਸ਼ਿਫਟਿੰਗ |
| unary operator | ਯੂਨਰੀ ਓਪਰੇਟਰ |
| binary operator | ਬਾਈਨਰੀ ਓਪਰੇਟਰ |

---

# Collections and Iteration

| English | Preferred Punjabi |
|---------|-------------------|
| iterable | ਇਟਰੇਬਲ |
| iterator | ਇਟਰੇਟਰ |
| loop | ਲੂਪ |
| iteration | ਇਟਰੇਸ਼ਨ |
| membership test | ਮੈਂਬਰਸ਼ਿਪ ਜਾਂਚ |
| sequence operations | ਕ੍ਰਮ ਕਾਰਵਾਈਆਂ |
| mapping operations | ਮੈਪਿੰਗ ਕਾਰਵਾਈਆਂ |

---

# Exceptions and Errors

| English | Preferred Punjabi |
|---------|-------------------|
| exception | ਅਪਵਾਦ |
| error | ਗਲਤੀ |
| traceback | ਟ੍ਰੇਸਬੈਕ |
| warning | ਚੇਤਾਵਨੀ |
| runtime error | ਰਨਟਾਈਮ ਗਲਤੀ |

---

# Modules and Libraries

| English | Preferred Punjabi |
|---------|-------------------|
| module | ਮੌਡਿਊਲ |
| package | ਪੈਕੇਜ |
| standard library | ਮਿਆਰੀ ਲਾਇਬ੍ਰੇਰੀ |
| library | ਲਾਇਬ੍ਰੇਰੀ |
| import | ਇੰਪੋਰਟ |
| built-in module | ਬਿਲਟ-ਇਨ ਮੌਡਿਊਲ |
| package index | ਪੈਕੇਜ ਇੰਡੈਕਸ |
| virtual environment | ਵਰਚੁਅਲ ਇਨਵਾਇਰਨਮੈਂਟ |

---

# String and Formatting Terms

| English | Preferred Punjabi |
|---------|-------------------|
| formatting | ਫਾਰਮੈਟਿੰਗ |
| string formatting | ਸਤਰ ਫਾਰਮੈਟਿੰਗ |
| interpolation | ਇੰਟਰਪੋਲੇਸ਼ਨ |
| formatted string literal | ਫਾਰਮੈਟ ਕੀਤੀ ਸਤਰ ਲਿਟਰਲ |
| f-string | f-string |
| placeholder | ਪਲੇਸਹੋਲਡਰ |
| template | ਟੈਂਪਲੇਟ |
| delimiter | ਡਿਲਿਮਿਟਰ |
| universal newlines | ਯੂਨੀਵਰਸਲ ਨਿਊਲਾਈਨਜ਼ |
| encoding | ਐਨਕੋਡਿੰਗ |
| decoding | ਡੀਕੋਡਿੰਗ |
| serialization | ਸੀਰੀਅਲਾਈਜ਼ੇਸ਼ਨ |
| deserialization | ਡੀਸੀਰੀਅਲਾਈਜ਼ੇਸ਼ਨ |

---

# Numeric Terms

| English | Preferred Punjabi |
|---------|-------------------|
| decimal | ਦਸ਼ਮਲਵ |
| hexadecimal | ਹੈਕਸਾਡੈਸੀਮਲ |
| octal | ਆਕਟਲ |
| binary | ਬਾਈਨਰੀ |
| precision | ਸ਼ੁੱਧਤਾ |
| rounding | ਗੋਲਾਈਕਰਨ |
| conversion | ਰੂਪਾਂਤਰਨ |
| approximation | ਅਨੁਮਾਨ |
| floating-point | ਫਲੋਟਿੰਗ-ਪੌਇੰਟ |
| binary fraction | ਬਾਈਨਰੀ ਭਿੰਨ |
| decimal fraction | ਦਸ਼ਮਲਵ ਭਿੰਨ |
| representation | ਪ੍ਰਤਿਨਿਧਿਤਾ |
| representation error | ਪ੍ਰਤਿਨਿਧਿਤਾ ਗਲਤੀ |

---

# Standard Library Terms

| English | Preferred Punjabi |
|---------|-------------------|
| thread | ਥ੍ਰੈਡ |
| threading | ਥ੍ਰੈਡਿੰਗ |
| queue | ਕਤਾਰ |
| lock | ਲਾਕ |
| semaphore | ਸੈਮਾਫੋਰ |
| event | ਇਵੈਂਟ |
| logging | ਲੌਗਿੰਗ |
| log message | ਲੌਗ ਸੁਨੇਹਾ |
| callback | ਕਾਲਬੈਕ |
| cache | ਕੈਸ਼ |
| garbage collection | ਗਾਰਬੇਜ ਕਲੇਕਸ਼ਨ |
| weak reference | ਕਮਜ਼ੋਰ ਰੈਫਰੈਂਸ |
| synchronization | ਸਿੰਕ੍ਰੋਨਾਈਜ਼ੇਸ਼ਨ |
| binary data | ਬਾਈਨਰੀ ਡਾਟਾ |
| record | ਰਿਕਾਰਡ |

---

# Documentation Terms

| English | Preferred Punjabi |
|---------|-------------------|
| tutorial | ਟਿਊਟੋਰਿਅਲ |
| documentation | ਦਸਤਾਵੇਜ਼ੀਕਰਨ |
| guide | ਮਾਰਗਦਰਸ਼ਿਕਾ |
| reference | ਸੰਦਰਭ |
| example | ਉਦਾਹਰਨ |
| explanation | ਵਿਆਖਿਆ |
| chapter | ਅਧਿਆਇ |
| section | ਭਾਗ |
| translation | ਅਨੁਵਾਦ |
| contributor | ਯੋਗਦਾਨਕਰਤਾ |
| validation | ਪ੍ਰਮਾਣਿਕਤਾ ਜਾਂਚ |
| terminology | ਪਰਿਭਾਸ਼ਿਕ ਸ਼ਬਦਾਵਲੀ |
| glossary | ਸ਼ਬਦਾਵਲੀ |
| style guide | ਸ਼ੈਲੀ ਮਾਰਗਦਰਸ਼ਿਕਾ |

---

# Documentation Workflow Terms

| English | Preferred Punjabi |
|---------|-------------------|
| translated message | ਅਨੁਵਾਦਿਤ ਸੁਨੇਹਾ |
| untranslated message | ਅਣਅਨੁਵਾਦਿਤ ਸੁਨੇਹਾ |
| fuzzy translation | ਅਸਪਸ਼ਟ ਅਨੁਵਾਦ |
| source string | ਸਰੋਤ ਸਤਰ |
| target string | ਲਕਸ਼ ਸਤਰ |
| validation check | ਪ੍ਰਮਾਣਿਕਤਾ ਜਾਂਚ |
| validation workflow | ਪ੍ਰਮਾਣਿਕਤਾ ਵਰਕਫਲੋ |
| translation workflow | ਅਨੁਵਾਦ ਵਰਕਫਲੋ |
| translated file | ਅਨੁਵਾਦਿਤ ਫਾਈਲ |
| completed file | ਪੂਰੀ ਕੀਤੀ ਫਾਈਲ |
| reviewer | ਸਮੀਖਿਆਕਾਰ |
| review | ਸਮੀਖਿਆ |
| proofreading | ਪ੍ਰੂਫਰੀਡਿੰਗ |
| synchronization | ਸਮਕਾਲੀਕਰਨ |

---

# Terms Commonly Left Untranslated

The following terms are widely recognized within the Python ecosystem and should normally remain in English unless there is a strong project-wide reason to translate them.

```text
Python
API
JSON
XML
HTML
HTTP
HTTPS
URL
Unicode
UTF-8
ASCII
Git
GitHub
Transifex
Linux
Windows
macOS
POSIX
CPython
PyPI
pip
venv
IDLE
REPL
```

---

# Common Python Keywords

Python language keywords must never be translated.

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

# Language Tag

The project uses the following IETF language tag for Punjabi:

```text
pa
```

This language tag is used throughout the repository, GitHub workflows, Transifex configuration, and CPython documentation builds.

---

# Consistency Rules

To maintain a consistent translation across the project:

- Always use glossary-approved terminology whenever an established translation exists.
- Do not introduce alternative translations for existing technical terms.
- Reuse terminology from previously completed translation files whenever possible.
- Function names, module names, class names, exception names, directives, roles, placeholders, and code identifiers must remain unchanged.
- When uncertain, prefer the terminology already used in completed translations rather than creating new variants.
- Follow the conventions described in `STYLE_GUIDE.md` for formatting, punctuation, and writing style.

Consistency across the entire documentation is more important than individual translation preferences.

---

# Glossary Maintenance

This glossary is a living document and should evolve as the Punjabi translation project continues to grow.

New terminology should be added only when:

- A previously untranslated technical term appears in the documentation.
- Contributors agree on a preferred translation.
- The terminology has been reviewed for consistency with existing translations.
- The term is expected to be reused across multiple documentation files.

When updating the glossary:

1. Verify that the term does not already exist under a different translation.
2. Use the same wording consistently across all translated files.
3. Update existing translations if a project-wide terminology change is adopted.
4. Review the glossary after major translation milestones to keep terminology current.

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

# Final Notes

This glossary defines the preferred terminology for the Punjabi (`pa`) translation of the Python documentation.

All contributors are encouraged to consult this glossary before translating new documentation and to update it whenever new project-approved terminology is established.

Using consistent terminology across the repository improves readability, simplifies reviews, reduces translation inconsistencies, and provides a high-quality documentation experience for Punjabi-speaking Python users.
