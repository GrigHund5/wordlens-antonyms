# Wordlens Wiktionary antonym list

`wordlens-wiktionary-antonyms.tsv` contains 416 English antonym pairs (822 rows, each pair in both directions where the reverse wasn't already supplied by WordNet). They're bundled in the Wordlens iOS app's `wordnet.sqlite` (rows in the `related` table with `source = 'wiktionary'`).

## Attribution
- **Source:** Wiktionary, https://en.wiktionary.org, by Wiktionary contributors. It was extracted with Wiktextract, as published by kaikki.org (https://kaikki.org/dictionary/English/).
- **Original license:** CC BY-SA 4.0 (also GFDL). See https://en.wiktionary.org/wiki/Wiktionary:Copyrights.

## Changes made
The pairs were filtered by Wordlens using `tools/extract_wiktionary_antonyms.py`. A pair is kept only when all of these hold:
- Both words are common single words.
- Both are Open English WordNet lemmas with the same part of speech.
- Both entries list each other.
- Neither sense is tagged slang, informal, dated, archaic, rare, technical, political or religious.
- The pair isn't in the Wordlens denylist and isn't already a WordNet antonym.

No Wiktionary definitions or other text are included.

## License
This list is licensed under **CC BY-SA 4.0** (`LICENSE`, https://creativecommons.org/licenses/by-sa/4.0/). You may share and adapt it, including commercially, if you give attribution and share adaptations under the same license.

The bundled `wordnet.sqlite` combines this list with Open English WordNet 2025 (CC BY 4.0, https://en-word.net). The combined related-words data is offered under CC BY-SA 4.0.
