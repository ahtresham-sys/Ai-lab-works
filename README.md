# Introduction to AI: Lab Works

Lab work for **Introduction to AI** (BS Robotics & AI, University of Lahore).

| Folder | Topic |
|---|---|
| `lab-02-web-scraping-eda/` | Web scraping, spaCy/TextBlob feature engineering, EDA, TF-IDF |
| `lab-03-text-image-features/` | Turning text and images into machine-readable features |
| `lab-04-regression-logistic/` | Linear and logistic regression (diabetes, housing, salary) |
| `lab-06-fastapi-diabetes-api/` | Serving a trained model with FastAPI |
| `lab-07-cnn-kernel-from-scratch/` | Convolution, ReLU, flatten, dense, softmax in NumPy |
| `cancer-app/` | Tumour classifier web app (FastAPI + sliders) |
| `diabetes-app/` | Diabetes predictor web app, live demo: https://diabetes-predictor-jwjc.onrender.com |
| `practice/` | Practice datasets and notebooks |

## Running the apps
```
cd cancer-app        # or diabetes-app
python -m pip install -r requirements.txt
python train.py      # cancer-app only
python -m uvicorn main:app --reload --port 8000
```
Educational projects only, not medical advice.
