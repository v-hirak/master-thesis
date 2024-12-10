# Dataset of Typological Language Properties

This dataset is part of my Master's Thesis project and contains a variety of properties for 212 languages included in the [FLORES+ dataset](https://github.com/openlanguagedata/flores). 

## Description of Columns

The data is aggregated in the `lang_data.csv` file. Below are the descriptions of each of the columns:

### Basic Taxonomic Properties

- `lang`: language ID from the [FLORES+ dataset](https://github.com/openlanguagedata/flores).
- `iso_code`: ISO-639-3 code.
- `wals_code`: code in the [WALS Database](https://wals.info/), available for 176 languages.
- `script`: language script extracted from the FLORES+ dataset.
- `variety`: glottocode found in the FLORES+ dataset.
- `name`: full name of the language from the FLORES+ dataset.
- `family`: language family as per WALS.
- `genus`: language genus as per WALS.

### Precomputed Typological Distances from English

Calculated using the [lang2vec library](https://github.com/antonisa/lang2vec). Available for all 212 languages.

- `d_gen`: genetic distance, represents the distance from English on the hypothesized Glottolog language tree.
- `d_geo`: geographic distance, calculated as the "great circle" distance between the English and a given language on the surface of the Earth.
- `d_syn`: syntactic distance from English, calculated as cosine distance between feature vectors derived from syntactic structures.
- `d_inv`: inventory distance from English, calculated as cosine distance between the phonological feature vectors derived from the [PHOIBLE](https://phoible.org/), [WALS](https://wals.info/), and [Ethnologue](https://www.ethnologue.com/) databases.
- `d_pho`: phonological distance from English, calculated as cosine distance between the phonological feature vectors derived from the [PHOIBLE](https://phoible.org/), [WALS](https://wals.info/), and [Ethnologue](https://www.ethnologue.com/) databases.
- `d_fea`: featural distance from English, calculated as cosine distance between feature vectors combining all five features described above.

### WALS Features

12 WALS features (20A-29A) from the "Morphology" category and one (81A) from the "Word Order" category. Feature values correspond to their order in the respective WALS features.

- `20A`: Fusion of Selected Inflectional Formatives. Available for 38 languages.
- `21A`: Exponence of Selected Inflectional Formatives. Available for 38 languages.
- `21B`: Exponence of Tense-Aspect-Mood Inflection. Available for 38 languages.
- `22A`: Inflectional Synthesis of the Verb. Available for 38 languages.
- `23A`: Locus of Marking in the Clause. Available for 46 languages.
- `24A`: Locus of Marking in Possessive Noun Phrases. Available for 46 languages.
- `25A`: Locus of Marking: Whole-language Typology. Available for 46 languages.
- `25B`: Zero Marking of A and P Arguments. Available for 46 languages.
- `26A`: Prefixing vs. Suffixing in Inflectional Morphology. Available for 109 languages.
- `27A`: Reduplication. Available for 77 languages.
- `28A`: Case Syncretism. Available for 45 languages.
- `29A`: Syncretism in Verbal Person/Number Marking. Available for 45 languages.
- `81A`: Order of Subject, Object and Verb. Available for 127 languages.