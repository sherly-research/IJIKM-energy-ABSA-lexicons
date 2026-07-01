# IJIKM Energy ABSA Lexical Resources

This repository provides the lexical resources used in the label-free aspect and sentiment discovery pipeline for Indonesian online public energy discussions.

The resources support preprocessing, aspect-level sentiment assignment, pragmatic cue handling, and energy-domain longitudinal filtering.

## Repository contents

- `lexicons/positive_clean.txt`: cleaned positive opinion lexicon adapted from Ramaprakoso's Indonesian sentiment keyword list.
- `lexicons/negative_clean.txt`: cleaned negative opinion lexicon adapted from Ramaprakoso's Indonesian sentiment keyword list.
- `lexicons/slangword.txt`: slang normalization dictionary adapted from SentiStrengthID and extended with corpus-specific variants.
- `lexicons/positive_energy_multiword_additions.txt`: manually curated positive energy-domain multiword expressions.
- `lexicons/negative_energy_multiword_additions.txt`: manually curated negative energy-domain multiword expressions.
- `lexicons/negator_true_energy.txt`: manually curated Indonesian negation cues.
- `lexicons/complaint_cues_energy.txt`: manually curated complaint-related cues for Indonesian energy discussions.
- `lexicons/emoticon_positive_lexicon_from_dataset.txt`: positive emoticon cues extracted and grouped from the corpus.
- `lexicons/emoticon_negative_lexicon_from_dataset.txt`: negative emoticon cues extracted and grouped from the corpus.
- `lexicons/emoticon_ambiguous_lexicon_from_dataset.txt`: ambiguous or pragmatic emoticon cues extracted and grouped from the corpus.
- `lexicons/custom_stopwords.txt`: manually curated stopwords and non-informative tokens.
- `lexicons/energy_domain_whitelist.txt`: energy-domain aspect whitelist used for longitudinal filtering.

## Original sources

The positive and negative opinion lexicons were initialized from Ramaprakoso's Indonesian sentiment keyword resources:

- https://github.com/ramaprakoso/analisis-sentimen/blob/master/kamus/positive_keyword.txt
- https://github.com/ramaprakoso/analisis-sentimen/blob/master/kamus/negative_keyword.txt

The slang normalization dictionary was adapted from SentiStrengthID:

- https://github.com/agusmakmun/SentiStrengthID/blob/master/id_dict/slangword.txt

Other resources were manually curated or extended based on corpus inspection of Indonesian and code-mixed online energy discussions.

## Multiword matching

Multiword expressions were prioritized before unigram matching. In the pipeline, longer expressions were checked first so that domain-specific expressions and sentiment cues were not fragmented into separate tokens.

## Citation

If you use these resources, please cite the related IJIKM manuscript.
