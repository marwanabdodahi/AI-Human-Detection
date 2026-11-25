# data/

| File | What it is |
|---|---|
| `open_qa.jsonl` | The original HC3 English Open QA file (1,187 questions). Copied here so the project runs without internet. |
| `train.csv` | 700 answers (350 questions) for training. |
| `val.csv` | 150 answers (75 questions) for choosing settings. |
| `test.csv` | 150 answers (75 questions) for the final score only. |

The three CSV files are made by `notebooks/00_data_baseline.ipynb`. Columns: `pair_id` (the question), `text` (the cleaned answer), `label` (0 = human, 1 = ChatGPT).

**Source:** Hello-SimpleAI, *Human ChatGPT Comparison Corpus* (Guo et al., 2023), English Open QA, revision `fdca6c0ff80c23431677544ee1feec2abd87dd5a`. https://huggingface.co/datasets/Hello-SimpleAI/HC3. License: CC BY-SA 4.0. The CSV files use the same license.

**Our changes:** whitespace and punctuation cleaning (to remove formatting shortcuts), removal of website error messages, deduplication, one human + one ChatGPT answer per question, a random sample of 500 questions (seed 42), and a split by question.
