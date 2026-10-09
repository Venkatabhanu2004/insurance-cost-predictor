# Insurance Cost Predictor
 An end-to-end machine learning project that predicts **annual health insurance costs** using customer demographics, lifestyle, health history, and policy-related features.  
 Built with **Random Forest**, a clean **src layout**, **Streamlit** for interactive UI, **Docker** for containerized deployment, and integrated **logging** for reproducibility and debugging.


---

## 🛠️ Tech Stack
- Python (pandas, scikit-learn, joblib)
- Random Forest Regressor
- Streamlit
- Docker
- Logging (Python `logging` module)

---

## 🚀 Run the Project with Docker

Make sure **Docker Desktop** is running.

### 1. Build the Docker Image
```bash
docker build -t insurance-predictor .

docker run -it insurance-predictor python train_pipeline.py

docker run -p 8501:8501 insurance-predictor streamlit run streamlit.py --server.port=8501 --server.address=0.0.0.0

 
