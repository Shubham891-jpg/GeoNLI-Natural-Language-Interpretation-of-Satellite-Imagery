# GeoNLI — Models

This directory is for storing model weights and checkpoints locally.

> ⚠️ **Do NOT commit model weights to Git.** They are excluded via `.gitignore`.

## Usage

Model weights should be downloaded separately (e.g., from Hugging Face Hub) and placed here, or loaded programmatically at runtime.

## Model Documentation

All model selection decisions should be documented in:

- `docs/model-selection.md` — rationale and comparison
- `docs/experiments/` — individual experiment logs

For each model, document:

- Model name and version
- Source / repository
- License
- Task (captioning / VQA / grounding)
- Model size and VRAM requirement
- Inference speed (measured, not estimated)
- Satellite imagery suitability (tested, not assumed)
