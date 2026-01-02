# Multilingual Usage Guidance

> Updated Date：2026.01.01<br/>Author：YQ之神<br/>Compatible Engine：DiffSinger<br/>Compatible Editor：OpenUTAU ≥ 0.1.547

## Overview

This voicebank supports following languages:

| Language | Tag  |                Recommended Phonemizer                 |             Supported input forms              |
| :------: | :--: | :---------------------------------------------------: | :--------------------------------------------: |
| Chinese  |  zh  |                       DIFFS-ZH                        | Hanzi (only when set as main language), pinyin |
| Japanese |  ja  |                       DIFFS-JA                        | Kana (only when set as main language), romaji  |
| English  |  en  | DIFFS-EN (with basic pronunciation prediction), DIFFS |                 English words                  |

## Cross-lingual control method

### Track-level control

Switch the phonemizer on the track to set the main language of the track.

### Note-level control

Lyrics of the supported forms of the main language of the track can be directly fill into the notes. To insert lyrics in other languages, a prefix with the language tag is required, i.e. `zh/ba`, `ja/to`, `en/hello`.

Note: this function finds the word or pronunciation directly in the dictionary. For this reason, hanzi, Japanese kana and English pronunciation prediction is unavailable if it is not the main language of the track.

### Phoneme-level control

Due to limits of the editor, all phonemes (except the global phonemes `AP` and `SP`) should be prefixed with their language tags, i.e. `zh/a`, `ja/o`, `en/eh`.

The following lyric form can be filled into notes to assign phoneme sequences directly: `[hh ax l ow]`. Prefixes of phonemes from the main language of the track can be omitted, while phonemes from other languages require full prefixes; phonemes tags in the phoneme panel can also be directly edited with prefixed full phoneme name.

## Attachments

- Chinese Pinyin Table
- Japanese Romaji Table
- English Phoneme Table