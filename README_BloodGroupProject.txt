
#  Blood Group Detection using Fingerprint Images

An AI-powered system that predicts a person's **blood group** using their **fingerprint image** through a deep learning model (EfficientNet), and provides **personalized health and nutrition recommendations** — all wrapped inside a secure and user-friendly **Streamlit web application**.

---

##  Overview

This project aims to simplify and speed up the blood group identification process using biometric data. Traditional blood testing is invasive and time-consuming — especially in emergencies. Our model leverages **fingerprint patterns** and a trained CNN model to detect the user's blood group instantly.

Built using:
- **TensorFlow/Keras (EfficientNet)**
- **Streamlit** for interface
- **OpenCV/PIL** for image handling
- **Secure login/register system** using `Streamlit session_state` and JSON-based auth

---

## Key Features

-  Predicts blood group from fingerprint image  
-  Personalized health suggestions based on blood type  
-  Clean UI built using Streamlit  
-  Login & Register system for user access control  
-  Works locally in the browser via `localhost`  
-  Fully modular backend for easy scaling or deployment  
-  Fast inference with EfficientNet for mobile-ready model architecture

---

## Technologies Used

| Area              | Tools / Frameworks                       |
|-------------------|------------------------------------------|
| Programming       | Python 3.10                              |
| Deep Learning     | TensorFlow, Keras, EfficientNet          |
| Image Handling    | OpenCV, Pillow (PIL)                     |
| Frontend          | Streamlit                                |
| Authentication    | JSON-based auth, `st.session_state`      |
| Model File        | `.h5` saved Keras model (EffNetB0)       |
| Data              | Fingerprint images labeled by blood type |

---

## Project Structure

```
├── app.py                  # Main Streamlit interface
├── auth.py                 # Login/Register functions
├── effnet.h5               # Trained model for blood group prediction
├── users.json              # Authenticated user database
├── data/                   # Fingerprint image dataset
├── cluster_1_0.BMP         # Sample image (test)
└── requirements.txt        # All dependencies
```

---

## 🛠️ How to Run the Project Locally

1. **Clone the Repository**
```bash
git clone https://github.com/your-username/blood-group-fingerprint.git
cd blood-group-fingerprint
```

2. **Create a Virtual Environment**
```bash
python -m venv venv
venv\Scripts\activate  # On Windows
```

3. **Install Required Packages**
```bash
pip install -r requirements.txt
```

If any error occurs, install manually:
```bash
pip install streamlit tensorflow-cpu==2.10 numpy==1.23.5 protobuf==3.20.3 pillow opencv-python
```

4. **Run the App**
```bash
streamlit run app.py
```

5. **Access the App**
Open browser and visit: `http://localhost:8501`

---

## 🔐 Default Credentials

```
Username: test
Password: 123
```

---

##  Blood Group Recommendations

Each predicted blood group will return:
- Suggested Fruits
- Recommended Vegetables
- Ideal Exercises

Example for `O+`:
- Fruits: Mango, Bananas
- Vegetables: Broccoli, Peppers
- Exercise: Running, Weightlifting

---

## Future Scope

- Deploy to **Streamlit Cloud** or **Heroku**
- Convert to `.exe` for offline use
- Add PDF download of result
- Add database for user history
- Extend to real-time fingerprint scanning

---

# Acknowledgments

Special thanks to open-source contributors and medical research data on blood group characteristics and dietary needs. Inspired by the need for faster blood group detection in critical care.

---

# Contact

**Author**: Jayanth Vadavalli  
**GitHub**: [@Jayyy0007](https://github.com/Jayyy0007)  
**Email**: jayanthvadavalli82@gmail.com 
**LinkedIn**: [https://www.linkedin.com/in/jayanth-vadavalli-591a2a312/)

---

#  License

This project is licensed under the MIT License — free to use, modify, and distribute with credit.
