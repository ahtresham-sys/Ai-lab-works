# Tumour Classifier: interactive ML web app

Train a model, serve it with FastAPI, explore it in the browser.

```
cancer_app/
├── train.py          trains the model, writes model.pkl + metadata.json
├── main.py           FastAPI backend (API + serves the page)
├── requirements.txt
└── static/
    ├── index.html    page
    ├── style.css
    └── app.js        sliders -> API calls -> live result
```

## Run

```
python -m pip install -r requirements.txt
python train.py
python -m uvicorn main:app --reload --port 8000
```

Open http://localhost:8000 (the app) or http://localhost:8000/docs (API docs).

## API

| Method | Path | Purpose |
|---|---|---|
| GET | /api/info | feature ranges + model accuracy |
| POST | /api/predict | `{"values": {"mean radius": 14, ...}}` -> label, probabilities, per-feature effects |
| GET | /api/health | health check |

Educational demo only, not for medical use.
