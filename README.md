# GeoNLI — Natural Language Interpretation of Satellite Imagery

A multimodal geospatial intelligence system that enables non-expert users to interact with satellite imagery through natural language.

## Core Capabilities

| Task | Input | Output |
|------|-------|--------|
| **Image Captioning** | Satellite image | Natural-language scene description |
| **Visual Question Answering (VQA)** | Image + question | Natural-language answer |
| **Visual Grounding** | Image + text query | Spatial regions (bounding boxes / masks) |

## Project Origin

Based on the **ISRO GeoNLI** problem presented at **Inter-IIT Tech Meet 14.0**.

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React + TypeScript + Tailwind CSS |
| Backend | Python + FastAPI |
| AI / ML | PyTorch + Hugging Face Transformers |
| CV | OpenCV (where needed) |

## Repository Structure

```
geo-nli/
├── frontend/          # React + TypeScript frontend
├── backend/           # FastAPI backend + AI services
├── data/              # Datasets (not committed — see data/README.md)
├── models/            # Model weights (not committed — see models/README.md)
├── docs/              # Architecture docs, experiments, research
├── tests/             # Integration / end-to-end tests
├── .env.example       # Environment variable template
├── .gitignore
├── LICENSE
└── README.md
```

## Getting Started

> 🚧 **Project is under active development.** Setup instructions will be added as components are implemented.

### Prerequisites

- Python 3.10+
- Node.js 18+
- npm or yarn

### Frontend

```bash
cd frontend
npm install
npm run dev
```

### Backend

```bash
cd backend
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
uvicorn app.main:app --reload
```

## Development Phases

1. **Phase 1** — Project skeleton, frontend + backend setup, image upload
2. **Phase 2** — MVP: one working VLM for basic VQA
3. **Phase 3** — Captioning, improved VQA, evaluation
4. **Phase 4** — Visual grounding, bounding boxes, counting
5. **Phase 5** — Large image handling, performance optimization
6. **Phase 6** — Evaluation, testing, documentation, deployment

## License

See [LICENSE](./LICENSE).
