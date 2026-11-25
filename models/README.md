# models/

Each notebook saves its trained model here:

| Folder | Made by | Size |
|---|---|---:|
| `Baseline/pipeline.joblib` | notebook 00 | 0.4 MB |
| `DistilBERT/` | notebook 01 | 269 MB |
| `DistilBERT-adapter/` | notebook 01 (LoRA bonus) | 3 MB |
| `ELECTRA-small/` | notebook 02 | 55 MB |
| `MiniLM/` | notebook 03 | 134 MB |
| `ALBERT/` | notebook 04 | 49 MB |
| `BERT-base/` | notebook 05 | 439 MB |
| `RoBERTa/` | notebook 06 | 503 MB |

The model folders are not in Git because they are too large (GitHub refuses files over 100 MB). Download them with the link in the main README, or run the notebooks again. The API (`api/app.py`) loads them from here.
