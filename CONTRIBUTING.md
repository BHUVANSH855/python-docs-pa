# Contributing

Thank you for helping translate the Python documentation into Punjabi. Typo fixes, new translations and reviews are all welcome.

## Ways to help

- **Translate or review** in [Transifex](https://explore.transifex.com/python-doc/python-newest/). Most of the work happens there, and you do not need a pull request. See [Transifex_Setup.md](Transifex_Setup.md).
- **Improve this repository** (guides, workflows, templates) with a pull request. See "Pull requests" below.
- **Report a problem** by opening an issue.

## Before you start

Read [STYLE_GUIDE.md](STYLE_GUIDE.md) and [GLOSSARY.md](GLOSSARY.md). [RULES.md](RULES.md) has the detailed rules for markup, placeholders and `.po` files. Use the glossary terms, and keep code, identifiers and reStructuredText markup unchanged.

## Translations

Translate and review in Transifex. Reviewed translations are pulled into this repository every day (see the [README](README.en.md)).

Please do not edit translations in the `.po` files here. The daily sync takes them from Transifex, so direct edits can be overwritten. If a `.po` file needs a fix that cannot be made in Transifex, ask a coordinator.

## Pull requests

For changes to the guides, workflows or templates:

1. Fork the repository, clone your fork and create a branch from `3.15`.
2. Make your change. Keep each pull request about one topic.
3. If you touched a `.po` file, run `msgfmt --check FILE.po`.
4. Push the branch and open a pull request against `3.15` with a clear description.

## Checks

CI runs `msgfmt --check` on every `.po` file for each push and pull request. It must pass.

```bash
msgfmt --check FILE.po    # required
sphinx-lint FILE.po       # optional, for larger changes
```

## Reviewing

A good review checks that:

- the meaning matches the English original,
- glossary terms are used,
- code, placeholders and markup are unchanged,
- the Punjabi reads naturally.

## Getting help

Open an issue, or ask one of the coordinators listed in the [README](README.en.md).

## License

Translations are contributed under the CC0 1.0 Universal license. By contributing, you agree that your contributions may be distributed under the same license.
