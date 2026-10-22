# Python ਦਸਤਾਵੇਜ਼ੀਕਰਨ ਦਾ ਪੰਜਾਬੀ ਅਨੁਵਾਦ

[English](README.en.md)

[Python ਦਸਤਾਵੇਜ਼ੀਕਰਨ](https://docs.python.org/) ਦਾ ਪੰਜਾਬੀ (ਗੁਰਮੁਖੀ, `pa`) ਅਨੁਵਾਦ।

- **ਪੜ੍ਹੋ:** <https://docs.python.org/pa/>
- **ਪ੍ਰਗਤੀ:** <https://translations.python.org/> (ਆਪਣੇ-ਆਪ ਅੱਪਡੇਟ ਹੁੰਦੀ ਹੈ)
- **ਅਨੁਵਾਦ ਅਤੇ ਸਮੀਖਿਆ:** [Transifex](https://explore.transifex.com/python-doc/python-newest/), ਭਾਸ਼ਾ ਪੰਜਾਬੀ (`pa`)
- **ਯੋਗਦਾਨ ਪਾਓ:** [CONTRIBUTING.md](CONTRIBUTING.md) ਵੇਖੋ (ਅੰਗਰੇਜ਼ੀ ਵਿੱਚ)

## ਅਨੁਵਾਦ ਕਿਵੇਂ ਕਰੀਏ?

1. Transifex ਉੱਤੇ [Python Documentation ਪ੍ਰੋਜੈਕਟ](https://explore.transifex.com/python-doc/python-newest/) ਖੋਲ੍ਹੋ।
2. "Join this project" ਬਟਨ ਦਬਾਓ। ਜੇ ਤੁਹਾਡਾ Transifex ਖਾਤਾ ਨਹੀਂ ਹੈ, ਤਾਂ ਬਣਾ ਲਓ।
3. ਪ੍ਰੋਜੈਕਟ ਦੇ ਪੰਨੇ ਉੱਤੇ ਪੰਜਾਬੀ (`pa`) ਚੁਣੋ।
4. ਕੋਆਰਡੀਨੇਟਰ ਵੱਲੋਂ ਮਨਜ਼ੂਰੀ ਮਿਲਣ ਤੋਂ ਬਾਅਦ ਕੋਈ ਰਿਸੋਰਸ ਚੁਣੋ ਅਤੇ [Transifex_Setup.md](Transifex_Setup.md) ਵਿੱਚ ਦਿੱਤੇ ਕਦਮਾਂ ਦੀ ਪਾਲਣਾ ਕਰੋ (ਅੰਗਰੇਜ਼ੀ ਵਿੱਚ)।
5. ਸਮੀਖਿਆਕਾਰ ਤੁਹਾਡੇ ਅਨੁਵਾਦਾਂ ਨੂੰ ਮਨਜ਼ੂਰ ਕਰਦੇ ਹਨ, ਅਤੇ ਰੋਜ਼ਾਨਾ ਸਮਕਾਲੀਕਰਨ ਨਾਲ ਉਹ ਇਸ ਰਿਪੋਜ਼ਟਰੀ ਵਿੱਚ ਆ ਜਾਂਦੇ ਹਨ। ਅਨੁਵਾਦਾਂ ਲਈ ਪੁੱਲ ਰਿਕਵੈਸਟ ਬਣਾਉਣ ਦੀ ਲੋੜ ਨਹੀਂ।

## ਇਹ ਕਿਵੇਂ ਕੰਮ ਕਰਦਾ ਹੈ?

ਅਨੁਵਾਦ Transifex ਵਿੱਚ ਲਿਖੇ ਅਤੇ ਸਮੀਖਿਆ ਕੀਤੇ ਜਾਂਦੇ ਹਨ। ਇੱਕ GitHub Actions ਵਰਕਫਲੋ ਹਰ ਰੋਜ਼ **ਸਮੀਖਿਆ ਕੀਤੇ ਗਏ** ਅਨੁਵਾਦਾਂ ਨੂੰ ਇਸ ਰਿਪੋਜ਼ਟਰੀ ਦੀਆਂ `3.13`, `3.14` ਅਤੇ `3.15` ਬ੍ਰਾਂਚਾਂ ਵਿੱਚ ਲਿਆਉਂਦਾ ਹੈ। ਜਿਨ੍ਹਾਂ ਸਤਰਾਂ ਦਾ ਅਨੁਵਾਦ ਹੋ ਚੁੱਕਾ ਹੈ ਪਰ ਸਮੀਖਿਆ ਨਹੀਂ ਹੋਈ, ਉਹ ਸਮੀਖਿਆ ਹੋਣ ਤੱਕ Transifex ਵਿੱਚ ਹੀ ਰਹਿੰਦੀਆਂ ਹਨ, ਇਸ ਲਈ ਉਹ ਅਜੇ ਰਿਪੋਜ਼ਟਰੀ ਵਿੱਚ ਨਹੀਂ ਹਨ।

ਹਰ ਪੁਸ਼ ਅਤੇ ਪੁੱਲ ਰਿਕਵੈਸਟ ਉੱਤੇ ਸਾਰੀਆਂ `.po` ਫ਼ਾਈਲਾਂ ਲਈ `msgfmt --check` ਚੱਲਦਾ ਹੈ। Python ਦਸਤਾਵੇਜ਼ੀਕਰਨ ਦੀ ਬਿਲਡ ਪੰਜਾਬੀ ਸਾਈਟ ਪ੍ਰਕਾਸ਼ਿਤ ਕਰਨ ਲਈ ਇਸ ਰਿਪੋਜ਼ਟਰੀ ਦੀ ਵਰਤੋਂ ਕਰਦੀ ਹੈ।

## ਮਾਰਗਦਰਸ਼ਿਕਾਵਾਂ

| ਫ਼ਾਈਲ | ਵਿਸ਼ਾ |
|------|-------|
| [CONTRIBUTING.md](CONTRIBUTING.md) | ਯੋਗਦਾਨ ਕਿਵੇਂ ਪਾਉਣਾ ਹੈ, ਜਾਂਚ ਕਿਵੇਂ ਕਰਨੀ ਹੈ ਅਤੇ ਤਬਦੀਲੀਆਂ ਕਿਵੇਂ ਭੇਜਣੀਆਂ ਹਨ |
| [Transifex_Setup.md](Transifex_Setup.md) | Transifex ਵਿੱਚ ਪਹਿਲੇ ਕਦਮ |
| [STYLE_GUIDE.md](STYLE_GUIDE.md) | ਅਨੁਵਾਦ ਦੀ ਸ਼ੈਲੀ ਅਤੇ ਨਿਯਮ |
| [RULES.md](RULES.md) | ਮਾਰਕਅੱਪ, ਪਲੇਸਹੋਲਡਰ ਅਤੇ `.po` ਫ਼ਾਈਲਾਂ ਲਈ ਵਿਸਤ੍ਰਿਤ ਨਿਯਮ |
| [GLOSSARY.md](GLOSSARY.md) | ਪਸੰਦੀਦਾ ਪੰਜਾਬੀ ਸ਼ਬਦਾਵਲੀ |

## ਕੋਆਰਡੀਨੇਟਰ

[@BHUVANSH855](https://github.com/BHUVANSH855), [@mohityadav8](https://github.com/mohityadav8) ਅਤੇ [@Yashraj-Jangra](https://github.com/Yashraj-Jangra)।

## ਲਾਇਸੈਂਸ

ਅਨੁਵਾਦ [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) ਲਾਇਸੈਂਸ ਅਧੀਨ ਯੋਗਦਾਨ ਵਜੋਂ ਦਿੱਤੇ ਜਾਂਦੇ ਹਨ।
