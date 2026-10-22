# Rules for Markup, Code and `.po` Files

These rules keep the translation valid and the documentation build working. For language and terminology, see [STYLE_GUIDE.md](STYLE_GUIDE.md) and [GLOSSARY.md](GLOSSARY.md).

We translate in Transifex (see [Transifex_Setup.md](Transifex_Setup.md)). The same rules apply to any `.po` file edited in this repository.

## Keep unchanged

Keep these exactly as in the English source:

- Python keywords, built-in names, and names of modules, packages, classes, functions, methods, attributes, exceptions and constants
- Variable, argument and parameter names in code
- C API names, command names, environment variables, file and directory names
- PEP numbers and version numbers (`3.12`, `Python 3.15`)
- URLs, anchors and reference identifiers
- Placeholders such as `%s`, `%d`, `%(name)s`, `{}`, `{0}`, `{name}` and `<filename>`

A name stays as it is even when a Punjabi spelling is possible. The words around a name are translated as usual.

## Code

- Do not change Python code: indentation, names, operators, imports, arguments or syntax.
- Do not change output, tracebacks or interactive sessions (the `>>>` and `...` prompts).
- Comments inside code may be translated if the meaning stays the same.
- Translate a string literal only when the English text clearly means the literal itself to be translated. It may also be data, output, an API value or an identifier.

## reStructuredText and Sphinx markup

- Keep roles and their targets: `:func:`, `:class:`, `:meth:`, `:exc:`, `:mod:`, `:ref:`, `:pep:` and so on.
- To show a Punjabi label, use the form with an explicit target and translate only the label. The target between `<` and `>` stays as in the English.
- Keep directives and their arguments (`.. note::`, `.. warning::`, `.. versionadded:: 3.12`, `.. code-block:: python`). Translate only the text inside them.
- Keep inline markup: `*italic*`, `**bold**`, ` ``code`` `, backticks, underscores and escaped characters.
- Keep the structure of the text (line breaks, lists, tables) as in the source.

```text
English: :ref:`function`
Wrong:   :ref:`ਫੰਕਸ਼ਨ`
Right:   :ref:`ਫੰਕਸ਼ਨ <function>`
```

## `.po` files

- Translate `msgstr` only. Never change `msgid`, the `#:` source references, the `#,` flags or the header. They come from the English source and are updated by the sync.
- If the English looks wrong, report it upstream. Do not fix it in the `.po` file.
- Keep the quoting, escapes and line breaks of multi-line strings valid.
- Do not add or remove `fuzzy` to skip a review. Check an uncertain translation and fix it first.
- Do not mix unrelated changes (formatting, metadata, other files) into a translation commit.

## Checks

Before sending a change, run:

```bash
msgfmt --check FILE.po
find . -name "*.po" -print0 | xargs -0 -n1 msgfmt --check -o /dev/null
git diff --check
git diff
```

The first two commands run `msgfmt` on one file and on all files. In `git diff`, confirm that no `msgid`, code, URL or placeholder changed and that there are no unrelated changes.

Optional: run `sphinx-lint FILE.po`, or build the HTML documentation locally as described in the [Developer's Guide](https://devguide.python.org/documentation/translations/translating/).
