
# AI Development Workflow – Assignment

**Course**: AI for Software Engineering  
**Duration**: 7 Days  
**Total Points**: 100

Overview
Predict student dropouts & hospital readmission risk using the full AI development lifecycle: problem definition, data prep, modeling, evaluation, deployment, monitoring, and ethics.

Repository Structure
- `docs/`: Contains PDF report and diagrams.
- `src/data_preprocessing.py`: Data loading and cleanup functions.
- `src/train_model.py`: Model training with train/val/test split and hyperparameter tuning.
- `src/evaluate_model.py`: Evaluation functions (confusion matrix, precision, recall, F1, ROC-AUC).
- `src/api/app.py`: Flask REST API for inference.
- `src/api/preprocess.py`: Text/data preprocessing used in the API.
- `src/api/requirements.txt`: Python dependencies (Flask, scikit-learn, XGBoost, etc.)

Setup Instructions
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r src/api/requirements.txt

Ethical and Critical Analysis

Discusses potential biases, fairness strategies, interpretability vs accuracy in healthcare, and resource-based model selection. Refer to Sections 3 and 4 in the PDF.

License

Code Snippets
- **`train_model.py`**: train XGBoost, save model with `joblib`.
- **`evaluate_model.py`**: load model, compute confusion matrix and metrics.
- **`app.py`**: Flask API using endpoints like `/predict_readmission`.

Next Steps
1. **Populate `docs/`**: export your PDF and include visuals.
2. **Implement code in `src/`** with clear comments.
3. **Test everything locally**, ensuring the API runs and returns sample predictions.
4. **Push to GitHub** and include a link in the PDF and README.
5. **Share** the PDF link as an article in PLP Academy Community.
