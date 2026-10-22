# Rules for Code, Markup and `.po` Files

These rules keep the documentation build working. For wording and terms, see [STYLE_GUIDE.md](STYLE_GUIDE.md) and [GLOSSARY.md](GLOSSARY.md).

We translate in Transifex ([Transifex_Setup.md](Transifex_Setup.md)). The same rules apply if you edit a `.po` file here.

## Leave these as they are

Copy the following from the English source without changes:

- Python keywords, built-in names, and the names of modules, packages, classes, functions, methods, attributes, exceptions and constants
- variable, argument and parameter names in code
- C API names, commands, environment variables, and file and folder names
- PEP numbers and version numbers, like `3.12` or `Python 3.15`
- URLs, anchors and reference names
- placeholders like `%s`, `%d`, `%(name)s`, `{}`, `{0}`, `{name}` and `<filename>`

A name stays as it is even if it could be written in Gurmukhi. Translate the words around it as usual.

## Code

Don't change Python code. That includes indentation, names, operators, imports and arguments. Output, tracebacks and interactive sessions (the `>>>` and `...` prompts) stay as they are too.

You can translate comments inside code as long as the meaning stays the same. Translate a string literal only if the English text clearly means the literal itself to be translated. It may also be data, output, an API value or an identifier.

## reStructuredText and Sphinx markup

Keep roles and their targets as they are: `:func:`, `:class:`, `:meth:`, `:exc:`, `:mod:`, `:ref:`, `:pep:` and so on.

If you want to show a Punjabi label, use the form with an explicit target and translate only the label. The target between `<` and `>` must stay as in the English.

```text
English: :ref:`function`
Wrong:   :ref:`ਫੰਕਸ਼ਨ`
Right:   :ref:`ਫੰਕਸ਼ਨ <function>`
```

Directives and their arguments also stay (`.. note::`, `.. warning::`, `.. versionadded:: 3.12`, `.. code-block:: python`). Translate only the text inside them. The same goes for inline markup such as `*italic*`, `**bold**` and ` ``code`` `. Keep the asterisks, backticks, underscores and escaped characters, and keep the structure of the text (line breaks, lists, tables).

## `.po` files

- Translate `msgstr` only. Never change `msgid`, the `#:` source references, the `#,` flags or the header. They come from the English source and are updated by the sync.
- If the English looks wrong, report it upstream. Don't fix it in the `.po` file.
- Keep the quotes, escapes and line breaks of multi-line strings valid.
- Don't add or remove `fuzzy` just to skip a review. Check an uncertain translation and fix it first.
- Don't mix unrelated changes (formatting, metadata, other files) into a translation commit.

## Checks

Before you send a change, run:

```bash
msgfmt --check FILE.po
find . -name "*.po" -print0 | xargs -0 -n1 msgfmt --check -o /dev/null
git diff --check
git diff
```

The first two run `msgfmt` on one file and on all files. In `git diff`, make sure that no `msgid`, code, URL or placeholder changed and that there are no unrelated changes.

You can also run `sphinx-lint FILE.po`, or build the HTML documentation locally as described in the [Developer's Guide](https://devguide.python.org/documentation/translations/translating/).
