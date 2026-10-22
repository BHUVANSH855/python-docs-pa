# Style Guide

This guide is about how we write the Punjabi. The rules for code and markup are in [RULES.md](RULES.md), and the agreed terms are in [GLOSSARY.md](GLOSSARY.md).

## The basics

Translate the meaning, not the words. The Punjabi should say what the English says, no more and no less. If two goals clash, accuracy wins over consistency, and consistency wins over style.

Write simple, natural Gurmukhi that a Punjabi-speaking programmer can read without effort. Keep the formal, teaching tone of the English documentation. Avoid slang and regional dialect, and don't translate word for word when the result sounds odd.

Never change the meaning of a technical term to make a sentence read better.

## Technical terms

For each term, go through these steps in order:

1. Use the term from the [glossary](GLOSSARY.md). Don't make up another one, and don't use two wordings in different files.
2. If the glossary doesn't have it, use a Punjabi word only if it means exactly the same thing.
3. If there is no such word, write the English word in Gurmukhi, for example ਰਿਪੋਜ਼ਟਰੀ.
4. Names, code and button labels stay in Latin script. So do the terms in the glossary's "Terms Commonly Left Untranslated" list.

After that, add the new term to the glossary. The steps are under "Adding or Changing a Term" there.

A few more things to watch:

- Look at the context first. The same English word can be a technical term, an everyday word or part of code. For the same reason, never run a find and replace for a term across many files.
- Other Python translations (Chinese, Japanese, Korean and so on) show how they dealt with a term. Use them for ideas, but don't copy their wording.
- An existing translation isn't wrong just because you would write it differently. Change it only when it is unclear, technically wrong or inconsistent.

## Machine translation

You can use it for a first draft, but a person has to read and fix every string. Typical problems are odd word order, wrong technical meaning, terms that don't match the glossary, and random jumps between English and Punjabi.

## Review

Before you approve a string in Transifex, check that:

- the meaning is the same as the English,
- it uses the glossary term,
- the Punjabi is natural, with correct grammar and spelling,
- roles, links, placeholders and code are untouched (see [RULES.md](RULES.md)).

Only reviewed strings reach this repository, so approve a string only when all four are true.

## Useful links

- [Python Developer's Guide: Translating](https://devguide.python.org/documentation/translations/translating/)
- [Python Developer's Guide: Style guide](https://devguide.python.org/documentation/style-guide/)
- [CPython glossary](https://docs.python.org/3/glossary.html)
