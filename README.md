# SmritiNER - SIH26003

Python/FastAPI hackathon MVP for an AI-assisted cognitive gaming and memory assistance platform for elderly users.

## Local run

```bash
python -m venv .venv
# Windows
.venv\\Scripts\\activate
# Linux/macOS
# source .venv/bin/activate

pip install -r requirements.txt
uvicorn app:app --reload
```

Open: http://127.0.0.1:8000/login

Demo accounts:
- Patient: `patient` / `1234`
- Caregiver: `caregiver` / `1234`

## Render deployment

This project includes `render.yaml` and uses Python 3.11.11 with pinned dependencies.

Render build command:
`pip install -r requirements.txt`

Render start command:
`uvicorn app:app --host 0.0.0.0 --port $PORT`

Health check:
`/health`

## Important

- No Windows-only packages such as `pywin32` are required.
- SQLite is used for this hackathon MVP. On a free cloud service, SQLite data should be treated as demo data and is not a production persistence strategy.
- Authentication uses demo plaintext passwords and is not production-grade security.
- Adaptive difficulty is a rule-based personalization engine, not a clinical diagnostic model.
- This prototype provides game-performance insights and is not a medical diagnosis/treatment tool.
