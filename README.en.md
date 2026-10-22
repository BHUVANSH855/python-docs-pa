# Python Documentation Translation — Punjabi (ਪੰਜਾਬੀ)

[ਪੰਜਾਬੀ](README.md)

Punjabi (Gurmukhi, `pa`) translation of the [Python documentation](https://docs.python.org/).

- **Read it:** <https://docs.python.org/pa/>
- **Progress:** <https://translations.python.org/> (updated automatically)
- **Translate and review:** [Transifex](https://explore.transifex.com/python-doc/python-newest/), language Punjabi (`pa`)
- **Contribute:** see [CONTRIBUTING.md](CONTRIBUTING.md)

## How do we translate?

1. Open the [Python Documentation project](https://explore.transifex.com/python-doc/python-newest/) on Transifex.
2. Click "Join this project". Create a Transifex account if you don't have one.
3. Select Punjabi (`pa`) on the project page.
4. After a coordinator approves your request, pick a resource and follow [Transifex_Setup.md](Transifex_Setup.md).
5. A reviewer approves your translations, and the daily sync brings them to this repository. You don't need to open a pull request for translations.

## How does it work?

Translations are written and reviewed in Transifex. A GitHub Actions workflow pulls the **reviewed** translations into this repository every day, into the `3.13`, `3.14` and `3.15` branches. Strings that are translated but not yet reviewed stay in Transifex until they are reviewed, so they are not in the repository yet.

Every push and pull request runs `msgfmt --check` on all `.po` files. The Python documentation build uses this repository to publish the Punjabi site.

## Guides

| File | Contents |
|------|----------|
| [CONTRIBUTING.md](CONTRIBUTING.md) | How to contribute, validate and submit changes |
| [Transifex_Setup.md](Transifex_Setup.md) | First steps in Transifex |
| [STYLE_GUIDE.md](STYLE_GUIDE.md) | Translation style and conventions |
| [RULES.md](RULES.md) | Detailed rules for markup, placeholders and `.po` files |
| [GLOSSARY.md](GLOSSARY.md) | Preferred Punjabi terminology |

## Coordinators

[@BHUVANSH855](https://github.com/BHUVANSH855), [@mohityadav8](https://github.com/mohityadav8) and [@Yashraj-Jangra](https://github.com/Yashraj-Jangra).

## License

Translations are contributed under the [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) license.
