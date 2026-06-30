# YOMI-Bench
YOMI-Bench is a benchmark for evaluating kanji reading ability in Japanese large language models (LLMs).
The dataset focuses on the ability to correctly infer the reading of a kanji character given its context.

# Data

## Dataset Structure & Tasks

- **kanji_reading_prediction**: Generate the correct reading of a target kanji in context.
  - **single**: Target kanji with a single valid reading.
  - **multiple**: Target kanji with multiple valid readings depending on context.

- **kanji_reading_qa**: Determine whether a proposed reading is correct (Yes/No).
  - **single**: Target kanji has a single valid reading.
  - **multiple**: Target kanji has multiple possible readings.

- **rhyme_selection**: Select the correct rhyming candidate from multiple choices.
  - **kanji**: Candidates are presented in kanji.
  - **hiragana**: Candidates are presented in hiragana.
 
- **rhyme_generation**: Generate a word or phrase that rhymes with the given input.

```text
YOMI-Bench/
├── readings.jsonl
│
├── tasks/
│   ├── kanji_reading_prediction/
│   │   ├── single/
│   │   │   ├── kanji_single_reading_hiragana_fewshot_0.jsonl
│   │   │   ├── kanji_single_reading_hiragana_fewshot_1.jsonl
│   │   │   ├── kanji_single_reading_hiragana_fewshot_2.jsonl
│   │   │   ├── kanji_single_reading_hiragana_fewshot_3.jsonl
│   │   │   └── kanji_single_reading_hiragana_fewshot_4.jsonl
│   │   └── multiple/
│   │       ├── kanji_multiple_reading_hiragana_fewshot_0.jsonl
│   │       ├── kanji_multiple_reading_hiragana_fewshot_1.jsonl
│   │       ├── kanji_multiple_reading_hiragana_fewshot_2.jsonl
│   │       ├── kanji_multiple_reading_hiragana_fewshot_3.jsonl
│   │       └── kanji_multiple_reading_hiragana_fewshot_4.jsonl
│   │
│   ├── kanji_reading_qa/
│   │   ├── single/
│   │   │   ├── kanji_single_reading_yesno_fewshot_0.jsonl
│   │   │   ├── kanji_single_reading_yesno_fewshot_1.jsonl
│   │   │   ├── kanji_single_reading_yesno_fewshot_2.jsonl
│   │   │   ├── kanji_single_reading_yesno_fewshot_3.jsonl
│   │   │   └── kanji_single_reading_yesno_fewshot_4.jsonl
│   │   └── multiple/
│   │       ├── kanji_multiple_reading_yesno_fewshot_0.jsonl
│   │       ├── kanji_multiple_reading_yesno_fewshot_1.jsonl
│   │       ├── kanji_multiple_reading_yesno_fewshot_2.jsonl
│   │       ├── kanji_multiple_reading_yesno_fewshot_3.jsonl
│   │       └── kanji_multiple_reading_yesno_fewshot_4.jsonl
│   │
│   ├── rhyme_selection/
│   │   ├── kanji/
│   │   │   ├── rhyme_selection_kanji_0.jsonl
│   │   │   ├── rhyme_selection_kanji_1.jsonl
│   │   │   ├── rhyme_selection_kanji_2.jsonl
│   │   │   ├── rhyme_selection_kanji_3.jsonl
│   │   │   └── rhyme_selection_kanji_4.jsonl
│   │   │
│   │   └── hiragana/
│   │       ├── kanji_selection_hiragana_0.jsonl
│   │       ├── kanji_selection_hiragana_1.jsonl
│   │       ├── kanji_selection_hiragana_2.jsonl
│   │       ├── kanji_selection_hiragana_3.jsonl
│   │       └── kanji_selection_hiragana_4.jsonl
│   │
│   └── rhyme_generation/
│       ├── rhyme_generation_hiragana_0.jsonl
│       ├── rhyme_generation_hiragana_1.jsonl
│       ├── rhyme_generation_hiragana_2.jsonl
│       ├── rhyme_generation_hiragana_3.jsonl
│       └── rhyme_generation_hiragana_4.jsonl
│   
│
└── README.md
```

# Citation
If you use this dataset in your research, please cite the following paper:

```
@article{mibayashi2026yomibench,
  title   = {YOMI-Bench: A Benchmark for Evaluating Kanji Reading and Phonological Understanding of LLMs for Japanese},
  author  = {Ryota Mibayashi and Hiroya Takamura and Hitomi Yanaka},
  journal = {arXiv preprint},
  year    = {2026},
  note    = {to appear}
}
```

# Contact
For questions, please contact mibayashi@people.kobe-u.ac.jp .

## License

This dataset is licensed under the
[Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/).
