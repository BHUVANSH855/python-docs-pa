# Transifex Guide

This guide helps new translators get started in Transifex. Translating and reviewing happen there, so you do not need Git, a fork or a pull request.

## Join the project

1. Create a Transifex account, or sign in, at <https://app.transifex.com/>.
2. Open the [Python Documentation project](https://explore.transifex.com/python-doc/python-newest/) and press "Join this project".
3. Choose Punjabi (`pa`) and wait for a coordinator to approve you. The coordinators are listed in the [README](README.en.md).
4. Ask a coordinator which resource to start with, so that two people do not work on the same one. A resource is one documentation file, for example `library-fileinput`.

If you cannot see Punjabi or your resource, ask a coordinator. Please do not create another project, language or resource.

## Translate

1. Open the project, choose Punjabi (`pa`) and open your resource in the editor.
2. Use the **Untranslated** filter to see the strings that still need translation.
3. Click a string. The editor shows the English source and a field for your Punjabi translation.
4. Press **Save**. Typing alone does not save the translation. Then go to the next string.

```text
Source:      Input and Output
Translation: ਇਨਪੁੱਟ ਅਤੇ ਆਉਟਪੁੱਟ
```

## Keep code and markup

Python documentation contains code and Sphinx markup, such as `print()`, `os.path`, `:func:`, `{name}`, `%s` and `.. code-block:: python`. Do not translate or change them. Translate only the text around them.

```text
Source:      It uses the :func:`print` function.
Translation: ਇਹ :func:`print` ਫੰਕਸ਼ਨ ਦੀ ਵਰਤੋਂ ਕਰਦਾ ਹੈ।
```

The details are in [RULES.md](RULES.md). Before translating a technical term, check [GLOSSARY.md](GLOSSARY.md). If the term is not there, follow the order in [STYLE_GUIDE.md](STYLE_GUIDE.md), and ask a coordinator if you are unsure. We want clear, natural, technically accurate Punjabi, not a word-for-word copy.

## Warnings and errors

Transifex checks a translation when you save it, for example for missing placeholders or changed markup. Read the message and fix the translation before saving again. If you do not understand it, ask a coordinator.

## When you finish a resource

- All strings are translated and saved.
- Code, placeholders and markup are unchanged.
- You followed the glossary and the style guide.

Then tell a coordinator. A reviewer approves the translations. Please do not mark translations as reviewed yourself unless you have been given reviewer permission.

## Review

Reviewers use the **Unreviewed** filter, check each string against the review points in [STYLE_GUIDE.md](STYLE_GUIDE.md), and mark it as reviewed. Ask a coordinator for reviewer permission.

## What happens next

Reviewed translations are pulled into this repository every day and published at <https://docs.python.org/pa/>. You do not need to upload `.po` files or open pull requests.

## If you get stuck

Ask a coordinator or open an issue if, for example:

- you cannot see Punjabi or your resource, or you cannot edit a string,
- a check fails and you do not understand why,
- you are unsure whether a word or markup should stay in English,
- an existing translation looks wrong,
- something looks like a Transifex configuration problem.

Please do not create a new project, resource, language or file to solve a problem yourself.
