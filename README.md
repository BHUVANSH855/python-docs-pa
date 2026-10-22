# Python ਦਸਤਾਵੇਜ਼ੀਕਰਨ ਦਾ ਪੰਜਾਬੀ ਅਨੁਵਾਦ

[English](README.en.md)

ਇਹ [Python ਦਸਤਾਵੇਜ਼ੀਕਰਨ](https://docs.python.org/) ਦਾ ਪੰਜਾਬੀ (ਗੁਰਮੁਖੀ, `pa`) ਅਨੁਵਾਦ ਹੈ।

- ਪੜ੍ਹੋ: <https://docs.python.org/pa/>
- ਕਿੰਨਾ ਅਨੁਵਾਦ ਹੋ ਚੁੱਕਾ ਹੈ: <https://translations.python.org/>
- ਅਨੁਵਾਦ ਅਤੇ ਸਮੀਖਿਆ: [Transifex](https://explore.transifex.com/python-doc/python-newest/) ਉੱਤੇ, ਭਾਸ਼ਾ ਪੰਜਾਬੀ (`pa`)
- ਯੋਗਦਾਨ ਪਾਉਣ ਲਈ: [CONTRIBUTING.md](CONTRIBUTING.md)

## ਅਨੁਵਾਦ ਕਿਵੇਂ ਕਰੀਏ?

1. Transifex ਉੱਤੇ [Python Documentation ਪ੍ਰੋਜੈਕਟ](https://explore.transifex.com/python-doc/python-newest/) ਖੋਲ੍ਹੋ ਅਤੇ "Join this project" ਬਟਨ ਦਬਾਓ। ਜੇ ਤੁਹਾਡਾ ਖਾਤਾ ਨਹੀਂ ਹੈ, ਤਾਂ ਪਹਿਲਾਂ ਬਣਾ ਲਓ।
2. ਪ੍ਰੋਜੈਕਟ ਦੇ ਪੰਨੇ ਉੱਤੇ ਪੰਜਾਬੀ (`pa`) ਚੁਣੋ। ਕੋਆਰਡੀਨੇਟਰ ਤੁਹਾਡੀ ਬੇਨਤੀ ਮਨਜ਼ੂਰ ਕਰਨਗੇ।
3. ਮਨਜ਼ੂਰੀ ਮਿਲਣ ਤੋਂ ਬਾਅਦ ਕੋਈ ਰਿਸੋਰਸ ਚੁਣੋ ਅਤੇ ਅਨੁਵਾਦ ਸ਼ੁਰੂ ਕਰੋ। ਪੂਰੇ ਕਦਮ [Transifex_Setup.md](Transifex_Setup.md) ਵਿੱਚ ਹਨ।
4. ਫਿਰ ਸਮੀਖਿਆਕਾਰ ਤੁਹਾਡੇ ਅਨੁਵਾਦ ਦੀ ਜਾਂਚ ਕਰਦੇ ਹਨ। ਮਨਜ਼ੂਰ ਹੋ ਜਾਣ ਤੋਂ ਬਾਅਦ ਇਹ ਆਪਣੇ-ਆਪ ਇਸ ਰਿਪੋਜ਼ਟਰੀ ਵਿੱਚ ਆ ਜਾਂਦਾ ਹੈ, ਇਸ ਲਈ ਪੁੱਲ ਰਿਕਵੈਸਟ ਬਣਾਉਣ ਦੀ ਲੋੜ ਨਹੀਂ।

## ਇਹ ਕਿਵੇਂ ਚੱਲਦਾ ਹੈ?

ਅਨੁਵਾਦ ਅਤੇ ਸਮੀਖਿਆ Transifex ਵਿੱਚ ਹੁੰਦੀ ਹੈ। ਹਰ ਰੋਜ਼ GitHub Actions ਦਾ ਇੱਕ ਵਰਕਫਲੋ ਸਮੀਖਿਆ ਹੋ ਚੁੱਕੇ ਅਨੁਵਾਦਾਂ ਨੂੰ ਇਸ ਰਿਪੋਜ਼ਟਰੀ ਦੀਆਂ `3.13`, `3.14` ਅਤੇ `3.15` ਬ੍ਰਾਂਚਾਂ ਵਿੱਚ ਲੈ ਆਉਂਦਾ ਹੈ। ਜਿਨ੍ਹਾਂ ਸਤਰਾਂ ਦੀ ਸਮੀਖਿਆ ਅਜੇ ਨਹੀਂ ਹੋਈ, ਉਹ Transifex ਵਿੱਚ ਹੀ ਰਹਿੰਦੀਆਂ ਹਨ।

ਹਰ ਪੁਸ਼ ਅਤੇ ਪੁੱਲ ਰਿਕਵੈਸਟ ਉੱਤੇ ਸਾਰੀਆਂ `.po` ਫ਼ਾਈਲਾਂ ਦੀ `msgfmt --check` ਨਾਲ ਜਾਂਚ ਹੁੰਦੀ ਹੈ। ਪੰਜਾਬੀ ਸਾਈਟ Python ਦਸਤਾਵੇਜ਼ੀਕਰਨ ਦੀ ਬਿਲਡ ਰਾਹੀਂ ਇਸੇ ਰਿਪੋਜ਼ਟਰੀ ਤੋਂ ਬਣਦੀ ਹੈ।

## ਹੋਰ ਫ਼ਾਈਲਾਂ

ਇਹ ਫ਼ਾਈਲਾਂ ਅੰਗਰੇਜ਼ੀ ਵਿੱਚ ਹਨ।

| ਫ਼ਾਈਲ | ਇਸ ਵਿੱਚ ਕੀ ਹੈ |
|------|-------------|
| [CONTRIBUTING.md](CONTRIBUTING.md) | ਯੋਗਦਾਨ ਕਿਵੇਂ ਪਾਉਣਾ ਹੈ |
| [Transifex_Setup.md](Transifex_Setup.md) | Transifex ਵਿੱਚ ਪਹਿਲੇ ਕਦਮ |
| [STYLE_GUIDE.md](STYLE_GUIDE.md) | ਅਨੁਵਾਦ ਦੀ ਭਾਸ਼ਾ ਅਤੇ ਸ਼ੈਲੀ |
| [RULES.md](RULES.md) | ਕੋਡ, ਮਾਰਕਅੱਪ ਅਤੇ `.po` ਫ਼ਾਈਲਾਂ ਦੇ ਨਿਯਮ |
| [GLOSSARY.md](GLOSSARY.md) | ਤਕਨੀਕੀ ਸ਼ਬਦਾਂ ਦੇ ਚੁਣੇ ਹੋਏ ਪੰਜਾਬੀ ਰੂਪ |

## ਕੋਆਰਡੀਨੇਟਰ

[@BHUVANSH855](https://github.com/BHUVANSH855), [@mohityadav8](https://github.com/mohityadav8) ਅਤੇ [@Yashraj-Jangra](https://github.com/Yashraj-Jangra)।

## ਲਾਇਸੈਂਸ

ਅਨੁਵਾਦ [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) ਲਾਇਸੈਂਸ ਅਧੀਨ ਯੋਗਦਾਨ ਵਜੋਂ ਦਿੱਤੇ ਜਾਂਦੇ ਹਨ।
