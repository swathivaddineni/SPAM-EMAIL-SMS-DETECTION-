# SPAM-EMAIL-SMS-DETECTION

# 📧 Image Spam Detector using Deep Learning

This project implements a binary image classification model to distinguish between **HAM** (non-spam) and **SPAM** images. The model uses **Fine-Tuned EfficientNetB0** and is deployed via a user-friendly Streamlit web interface.

## ⚙️ Repository Contents

| File | Description |

| `Spam_Detection_Project.ipynb` | The primary Google Colab notebook containing all setup, training, and deployment code. |
| `fixed_model.h5` | The trained **EfficientNetB0** model weights used for inference. |
| `best_threshold.pkl` | The calculated optimal probability threshold. |
| `app.py` | The complete Streamlit application script for the web interface. |
| `requirements.txt` | List of all Python packages required to run the project. |

## 🚀 Getting Started

The project can be run in two ways: via Google Colab (recommended) or locally.

### Option 1: Run via Google Colab (Recommended)

1.  **Open the Notebook:** Click on the `Spam_Detection_Project.ipynb` file in this repository and select **"Open in Colab."**
2.  **Execute Cells:** Run all cells sequentially. The final cell will handle deployment.
3.  **Note:** Ensure the data download and aggressive fine-tuning steps have been completed to use the most accurate model.

### Option 2: Local Deployment

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/swathivaddineni/SPAM-EMAIL-SMS-DETECTION-/new/main?readme=1]
    cd YOUR_REPO_NAME
    ```
2.  **Install Dependencies:** It is highly recommended to use a virtual environment.
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run Streamlit:**
    ```bash
    streamlit run app.py
    ```
    The application will launch iN your browser (usually at http://localhost:8501).

## 💡 Model Summary

The final model is an **EfficientNetB0** that was fine-tuned for high accuracy on image spam detection, specifically balanced against the public HAM dataset. The decision threshold is **hardcoded to $0.5$** for simplicity and robustness in deployment.
