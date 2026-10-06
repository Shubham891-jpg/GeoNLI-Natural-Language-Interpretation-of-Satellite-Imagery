# GeoNLI — Data

This directory is for datasets used in the project.

> ⚠️ **Do NOT commit large datasets to Git.** Use `.gitignore` to exclude them.

## Expected Structure

```
data/
├── raw/            # Original unprocessed data
├── processed/      # Cleaned / preprocessed data
├── images/         # Sample satellite images for testing
└── README.md
```

## Dataset Documentation

For every dataset used, document the following in `docs/datasets/`:

- Name
- Source URL
- License
- Task (captioning / VQA / grounding / detection)
- Format
- Number of samples used
- Preprocessing applied
- Train / validation / test split
- Known limitations
