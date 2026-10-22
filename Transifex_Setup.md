# Transifex Guide

This page shows new translators how to start in Transifex. You do all the work there, so you don't need Git, a fork or a pull request.

## Join the project

1. Create a Transifex account, or sign in, at <https://app.transifex.com/>.
2. Open the [Python Documentation project](https://explore.transifex.com/python-doc/python-newest/) and click "Join this project".
3. Choose Punjabi (`pa`). A coordinator will approve your request. The coordinators are listed in the [README](README.en.md).
4. Ask a coordinator which resource to start with, so that two people don't work on the same one. A resource is one documentation file, for example `library-fileinput`.

If you can't see Punjabi or your resource, ask a coordinator. Please don't create another project, language or resource.

## Translate

1. Open the project, choose Punjabi (`pa`) and open your resource in the editor.
2. Use the **Untranslated** filter to see what still needs translating.
3. Click a string. The editor shows the English text and a field for your Punjabi translation.
4. Click **Save**. Typing alone doesn't save it. Then move on to the next string.

```text
Source:      Input and Output
Translation: ਇਨਪੁੱਟ ਅਤੇ ਆਉਟਪੁੱਟ
```

## Code and markup

The documentation contains code and Sphinx markup, like `print()`, `os.path`, `:func:`, `{name}`, `%s` and `.. code-block:: python`. Leave these as they are and translate only the text around them.

```text
Source:      It uses the :func:`print` function.
Translation: ਇਹ :func:`print` ਫੰਕਸ਼ਨ ਦੀ ਵਰਤੋਂ ਕਰਦਾ ਹੈ।
```

[RULES.md](RULES.md) has the details. Before you translate a technical term, look it up in [GLOSSARY.md](GLOSSARY.md). If it isn't there, follow the steps in [STYLE_GUIDE.md](STYLE_GUIDE.md), and ask a coordinator if you're still unsure. We want Punjabi that is clear and correct, not a word-for-word copy.

## Warnings

Transifex checks a translation when you save it, for example for missing placeholders or changed markup. Read the message and fix the translation before you save it again. If you don't understand the message, ask a coordinator.

## When you finish a resource

Make sure that all strings are translated and saved, that code, placeholders and markup are unchanged, and that you followed the glossary and the style guide. Then tell a coordinator. A reviewer will approve your translations. Don't mark them as reviewed yourself unless you have reviewer permission.

## Reviewing

Reviewers use the **Unreviewed** filter, check each string against the [review checklist](STYLE_GUIDE.md#review) and mark it as reviewed. Ask a coordinator for reviewer permission.

## What happens next

Reviewed translations are copied into this repository every day and published at <https://docs.python.org/pa/>. You don't need to upload `.po` files or open pull requests.

## If you get stuck

Ask a coordinator or open an issue if:

- you can't see Punjabi or your resource, or you can't edit a string,
- a check fails and you don't know why,
- you're not sure if a word or markup should stay in English,
- an existing translation looks wrong,
- something looks like a Transifex setup problem.

Please don't create a new project, resource, language or file to fix it yourself.
