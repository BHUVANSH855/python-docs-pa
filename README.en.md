# Punjabi translation of the Python documentation

[ਪੰਜਾਬੀ](README.md)

This is the Punjabi (Gurmukhi, `pa`) translation of the [Python documentation](https://docs.python.org/).

- Read it: <https://docs.python.org/pa/>
- See how much is translated: <https://translations.python.org/>
- Translate and review: [Transifex](https://explore.transifex.com/python-doc/python-newest/), language Punjabi (`pa`)
- Contribute: [CONTRIBUTING.md](CONTRIBUTING.md)

## How to translate

1. Open the [Python Documentation project](https://explore.transifex.com/python-doc/python-newest/) on Transifex and click "Join this project". You need a Transifex account, so create one if you don't have it yet.
2. Choose Punjabi (`pa`) on the project page. A coordinator will approve your request.
3. Pick a resource and start translating. [Transifex_Setup.md](Transifex_Setup.md) explains the steps.
4. A reviewer checks your translation. Once it's approved, it reaches this repository by itself, so you don't need a pull request.

## How it works

We translate and review in Transifex. Every day a GitHub Actions workflow copies the reviewed translations into the `3.13`, `3.14` and `3.15` branches of this repository. Strings that are translated but not yet reviewed stay in Transifex.

Each push and pull request runs `msgfmt --check` on all `.po` files. The Python documentation build then uses this repository to publish the Punjabi site.

## Other files

| File | What's in it |
|------|--------------|
| [CONTRIBUTING.md](CONTRIBUTING.md) | How to contribute |
| [Transifex_Setup.md](Transifex_Setup.md) | First steps in Transifex |
| [STYLE_GUIDE.md](STYLE_GUIDE.md) | Language and style of the translation |
| [RULES.md](RULES.md) | Rules for code, markup and `.po` files |
| [GLOSSARY.md](GLOSSARY.md) | The agreed Punjabi technical terms |

## Coordinators

[@BHUVANSH855](https://github.com/BHUVANSH855), [@mohityadav8](https://github.com/mohityadav8) and [@Yashraj-Jangra](https://github.com/Yashraj-Jangra).

## License

Translations are contributed under the [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) license.
