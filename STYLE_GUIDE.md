# Style Guide

This guide explains how we write the Punjabi (`pa`) translation of the Python documentation. Rules for markup, code, placeholders and `.po` files are in [RULES.md](RULES.md). Approved terms are in [GLOSSARY.md](GLOSSARY.md).

## Principles

- We translate the meaning, not the words. The Punjabi must say exactly what the English says.
- Technical accuracy comes first, then consistency, then style.
- We write clear, natural Punjabi (Gurmukhi) that a Punjabi-speaking programmer can read easily.
- We never change the meaning of a technical term.

## Tone

- Formal, educational and clear, like the English documentation.
- No slang, no regional dialect, and no word-for-word translation that sounds unnatural.
- When in doubt: clarity over literal wording, consistency over personal preference, accuracy over style.

## Terminology

For every technical term we follow this order:

1. Use the term from [GLOSSARY.md](GLOSSARY.md). Do not create an alternative, and do not switch wording between files.
2. If the term is not listed, use a Punjabi word only when it has exactly the same technical meaning.
3. If there is no such Punjabi word, write the English word in Gurmukhi (transliteration).
4. Proper names, code and UI button labels stay in Latin script. So do the terms listed under "Terms Commonly Left Untranslated" in the glossary.

Then add the new term to the glossary, as described under "Adding or Changing a Term" there.

Please also:

- Check the context. The same English word can be a technical term, an ordinary word or part of code. Never run a find-and-replace for a term over many files.
- Look at other Python translations (for example Chinese, Japanese or Korean) to see how they handle a term, but do not copy their wording.
- Do not rewrite an existing translation only because you prefer another wording. Change it only for a clear language, technical or consistency reason.

## Machine translation

We use machine translation only as a first draft. A person must read and correct every string. Watch for unnatural word order, wrong technical meanings, inconsistent terms and unexplained switching between English and Punjabi.

## Review

Reviewers in Transifex check each string for:

- **Meaning:** it says the same as the English.
- **Terminology:** it uses the glossary term.
- **Punjabi:** it is natural, with correct grammar and spelling.
- **Markup:** roles, links, placeholders and code are intact (see [RULES.md](RULES.md)).

Only reviewed strings reach this repository, so approve a string only when it passes all four.

## References

- [Python Developer's Guide: Translating](https://devguide.python.org/documentation/translations/translating/)
- [Python Developer's Guide: Style guide](https://devguide.python.org/documentation/style-guide/)
- [CPython glossary](https://docs.python.org/3/glossary.html)
