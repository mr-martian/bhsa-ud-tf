# bhsa-ud-tf
Text-Fabric modules for UD Ancient Hebrew data

This repository houses an extension to the [BHSA](https://github.com/etcbc/bhsa) dataset generated from the [Universal Dependencies Ancient Hebrew treebank](https://github.com/UniversalDependencies/UD_Ancient_Hebrew-PTNK/).

It adds the following features:
- `deprel`
  - [UD dependency relation](https://universaldependencies.org/u/dep/)
- `head` (edge)
  - head word of this word
  - this will be a self-loop in the case of prepositions which are dependent on their pronominal suffixes
- `macula`
  - corresponding ID in the [MACULA](https://github.com/Clear-Bible/macula-hebrew/) dataset
- `prs_deprel`
  - same as `deprel` but for pronominal suffixes
- `prs_head` (edge)
  - same as `edge` but for pronominal suffixes
- `prs_macula`
  - same as `macula` but for pronominal suffixes
- `sdbh`
  - (mostly) disambiguated ID in MARBLE's [Semantic Dictionary of Biblical Hebrew](https://marble.bible/dictionary)
  - this will be a comma-separated list if ambiguity remains
- `strongs`
  - Number of the word root in Strong's Concordance
  - MACULA assigns non-numeric values to function words (conjunctions, prefixed prepositions) which are not listed in the original concordance
- `upos`
  - [Universal part-of-speech tag](https://universaldependencies.org/u/pos/)
