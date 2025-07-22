# 👁️‍🗨️ Myopia Risk Profiler

A full-stack application using **React.js**, **Flask**, and **Machine Learning** to help individuals assess their risk of developing myopia through interactive vision tests and lifestyle analysis.

---

## 📌 Table of Contents

- [Overview](#overview)  
- [Features](#features)  
- [Tech Stack](#tech-stack)  
- [Architecture](#architecture)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Model Training & Inference](#model-training--inference)  
- [Contributing](#contributing)  
- [License](#license)  
- [Contact](#contact)

---

## 📝 Overview

**Myopia Risk Profiler** is a smart, responsive web platform designed to collect vision and lifestyle data from users, then analyze it using machine learning to predict the likelihood of developing myopia. It combines a React frontend with a Flask backend and ML model integration.

---

## ✅ Features

- 🧪 **Vision tests** to simulate standard eye exams  
- 📋 **Lifestyle questionnaire** collecting screen time, outdoor activity, etc.  
- 🤖 **ML risk prediction** providing personalized myopia insights  
- 🧩 **Modular full-stack architecture** using REST APIs  
- 📱 **Responsive UI** that works across devices

---

## 🛠 Tech Stack

| Layer       | Technologies                                  |
|-------------|-----------------------------------------------|
| Frontend    | React.js, HTML5, CSS3, JavaScript             |
| Backend     | Flask, Python                                 |
| ML Model    | scikit-learn / TensorFlow / PyTorch (custom)  |
| Communication | RESTful APIs (JSON)                        |
| Deployment  | Docker (optional), GitHub, Heroku/AWS-ready   |

---

## 🧱 Architecture

```
[React Frontend] ↔ (REST API) ↔ [Flask Backend + ML Model]
```

### 📡 Data Flow:

1. **Frontend**: React gathers survey + vision test data → sends to backend.  
2. **Backend**: Flask receives data → preprocesses → forwards to ML model.  
3. **Model**: Processes features → returns a risk probability.  
4. **Response**: Flask sends the risk score → React displays insights.

---

## ⚙️ Installation

### Prerequisites:

- [Node.js](https://nodejs.org/) (v14+)
- [Python](https://www.python.org/) 3.8+
- [Git](https://git-scm.com/)

### Clone the Repository

```bash
git clone https://github.com/himanshukumar4751/Myopia_Detection.git
cd Myopia_Detection
```

### Set up the Backend (Flask + ML)

```bash
cd backend
python -m venv venv
# For Windows:
venv\Scripts\activate
# For macOS/Linux:
source venv/bin/activate

pip install -r requirements.txt
```

### Set up the Frontend (React)

```bash
cd ../frontend
npm install
npm run build  # Builds production-ready React files
```

---

## 🚀 Usage

### Run locally in development mode

```bash
# Backend (Flask API)
cd backend
flask run    # Runs on http://127.0.0.1:5000

# Frontend (React)
cd ../frontend
npm start    # Opens http://localhost:3000
```

- Open the site in your browser.
- Complete the vision and lifestyle inputs.
- Click submit to view your personalized myopia risk prediction.

---

## 🧠 Model Training & Inference

- **Model Directory**: `/backend/model/`
- **Training Script**: `train_model.py`
  - Loads preprocessed data
  - Trains a classifier/regressor
  - Saves model as `.pkl` or `.h5`
- **Prediction**: Flask serves a `/predict` API endpoint
  - Accepts JSON input from React
  - Loads the saved model
  - Returns prediction as a JSON response

---

## 🤝 Contributing

We welcome all contributions! Here's how you can help:

1. **Fork** the repository  
2. Create a **feature branch**:  
   ```bash
   git checkout -b feature/my-feature
   ```
3. **Commit your changes**:  
   ```bash
   git commit -m "Add awesome feature"
   ```
4. **Push the branch**:  
   ```bash
   git push origin feature/my-feature
   ```
5. **Open a Pull Request**

---

## 📄 License

This project is licensed under the **MIT License**.  
See the [LICENSE](./LICENSE) file for full text.

---

## 📬 Contact

**Maintainer**: Himanshu Kumar  
📧 Email: [himanshukumar4751@gmail.com](mailto:himanshukumar4751@gmail.com)  
🔗 GitHub: [@himanshukumar4751](https://github.com/himanshukumar4751)

---

## ⭐ Support

If you find this project helpful, please **star** the repository and share it with others!

```bash
# Add this README to your repo and commit
git add README.md
git commit -m "Add complete professional README"
git push
```

---
