# Lexicon Sources and Adaptation

This document describes the lexical resources used in the IJIKM label-free ABSA pipeline.

## Sentiment lexicons

The positive and negative opinion lexicons were initialized from Ramaprakoso's Indonesian sentiment keyword lists. The lists were cleaned and adapted to the Indonesian energy-discussion corpus.

Original sources:

- Positive keyword list: https://github.com/ramaprakoso/analisis-sentimen/blob/master/kamus/positive_keyword.txt
- Negative keyword list: https://github.com/ramaprakoso/analisis-sentimen/blob/master/kamus/negative_keyword.txt

## Slang normalization

The slang normalization dictionary was adapted from SentiStrengthID and extended with corpus-specific informal variants.

Original source:

- SentiStrengthID slangword dictionary: https://github.com/agusmakmun/SentiStrengthID/blob/master/id_dict/slangword.txt

## Manually curated resources

The following resources were manually curated or extended through corpus inspection:

- `positive_energy_multiword_additions.txt`
- `negative_energy_multiword_additions.txt`
- `negator_true_energy.txt`
- `complaint_cues_energy.txt`
- `emoticon_positive_lexicon_from_dataset.txt`
- `emoticon_negative_lexicon_from_dataset.txt`
- `emoticon_ambiguous_lexicon_from_dataset.txt`
- `custom_stopwords.txt`
- `energy_domain_whitelist.txt`

These resources were designed for Indonesian and code-mixed public discussions on energy issues.

## Energy-domain whitelist

The energy-domain whitelist was used for longitudinal filtering of energy-related aspect terms. It includes terms related to electricity, fuels, generation technologies, renewable energy, nuclear energy, and energy institutions.

## Notes on reuse

Some resources are adapted from existing public repositories. Users should consult the original repositories for their licensing and usage terms.
