# YOMI-Bench
YOMI-Bench is a benchmark for evaluating kanji reading ability in Japanese large language models (LLMs).
The dataset focuses on the ability to correctly infer the reading of a kanji character given its context.

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
│   │       ├── kanji_multi_reading_yesno_fewshot_0.jsonl
│   │       ├── kanji_multi_reading_yesno_fewshot_1.jsonl
│   │       ├── kanji_multi_reading_yesno_fewshot_2.jsonl
│   │       ├── kanji_multi_reading_yesno_fewshot_3.jsonl
│   │       └── kanji_multi_reading_yesno_fewshot_4.jsonl
│   │
│   ├── rhyme_generation/
│   │   ├── rhyme_generation_hiragana_0.jsonl
│   │   ├── rhyme_generation_hiragana_1.jsonl
│   │   ├── rhyme_generation_hiragana_2.jsonl
│   │   ├── rhyme_generation_hiragana_3.jsonl
│   │   └── rhyme_generation_hiragana_4.jsonl
│   │
│   └── rhyme_selection/
│       ├── kanji/
│       │   ├── rhyme_selection_kanji_0.jsonl
│       │   ├── rhyme_selection_kanji_1.jsonl
│       │   ├── rhyme_selection_kanji_2.jsonl
│       │   ├── rhyme_selection_kanji_3.jsonl
│       │   └── rhyme_selection_kanji_4.jsonl
│       │
│       └── hiragana/
│           ├── kanji_selection_hiragana_0.jsonl
│           ├── kanji_selection_hiragana_1.jsonl
│           ├── kanji_selection_hiragana_2.jsonl
│           ├── kanji_selection_hiragana_3.jsonl
│           └── kanji_selection_hiragana_4.jsonl
│
└── README.md
