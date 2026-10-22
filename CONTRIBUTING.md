# Contributing

Thanks for helping with the Punjabi translation of the Python documentation. There are three ways to help: translate or review strings, improve something in this repository, or report a problem.

## Translating and reviewing

This happens in [Transifex](https://explore.transifex.com/python-doc/python-newest/), and you don't need a pull request for it. [Transifex_Setup.md](Transifex_Setup.md) shows how to start. Please read the [style guide](STYLE_GUIDE.md) and the [glossary](GLOSSARY.md) first, and look at [RULES.md](RULES.md) for what has to stay unchanged. If you review, follow the [review checklist](STYLE_GUIDE.md#review).

Reviewed translations are copied into this repository every day (the [README](README.en.md) explains how). That's why you shouldn't edit translations in the `.po` files here: the next sync can overwrite your change. If a `.po` file needs a fix that can't be made in Transifex, ask a coordinator.

## Changing this repository

Pull requests are for the guides, the workflows and the templates.

1. Fork the repository, clone your fork and create a branch from `3.15`.
2. Make your change. Keep each pull request to one topic.
3. If you changed a `.po` file, run `msgfmt --check FILE.po`.
4. Push the branch and open a pull request against `3.15`. Say what you changed and why.

CI runs `msgfmt --check` on every `.po` file for each push and pull request, and it has to pass. For bigger changes, `sphinx-lint FILE.po` is a useful extra check.

## Questions and problems

Open an issue, or ask one of the coordinators listed in the [README](README.en.md).

## License

Translations are contributed under the CC0 1.0 Universal license. By contributing, you agree that your contributions may be distributed under the same license.
