# GeoNLI — Backend

Python + FastAPI backend for the GeoNLI system.

## Setup

```bash
python -m venv .venv
.venv\Scripts\activate        # Windows
# source .venv/bin/activate   # Linux/Mac
pip install -r requirements.txt
uvicorn app.main:app --reload
```

## Structure

```
app/
├── api/
│   └── routes/        # FastAPI route handlers
├── ai/
│   ├── captioning/    # Image captioning models & logic
│   ├── vqa/           # Visual question answering models & logic
│   └── grounding/     # Visual grounding models & logic
├── services/          # Business logic & orchestration
├── schemas/           # Pydantic request/response schemas
├── core/              # App config, settings, startup
└── utils/             # Shared utilities
```

## API Endpoints (PROPOSED)

| Method | Endpoint | Purpose |
|--------|----------|---------|
| GET | `/api/health` | Health check |
| POST | `/api/upload` | Upload satellite image |
| POST | `/api/caption` | Generate image caption |
| POST | `/api/vqa` | Visual question answering |
| POST | `/api/ground` | Visual grounding |

## Status

🚧 Under development — skeleton structure created.
