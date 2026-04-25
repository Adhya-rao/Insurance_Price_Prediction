# 🏥 Insurance Price Prediction App

A simple and interactive **Machine Learning web application** built using *Streamlit* to predict insurance charges based on user inputs like age, BMI, smoking habits, and more.

---

## 📌 Project Overview
This project predicts **medical insurance cost** using a trained ML model.  
Users can enter their details, and the app will estimate the **insurance price instantly**.

---

## 🚀 Live Demo
👉 https://insurancepriceprediction-syze7zmzrenybsnc5ibz9t.streamlit.app/

---

## 🧠 Technologies Used
* Python  
* Streamlit  
* Scikit-learn  
* Pandas  
* NumPy  
* Seaborn  
* Pickle  

---

## 📂 Features
* User-friendly UI using Streamlit  
* Real-time prediction  
* Input validation (age, BMI, children, etc.)  
* Encoded categorical variables (gender, smoker, region)  
* Scaled numerical features  
* ML model integration  

---

## 📊 Input Parameters
* **Age** → User age (1–100)  
* **Gender** → Male / Female  
* **BMI** → Body Mass Index (10–80)  
* **Smoker** → Yes / No  
* **Children** → Number of children (0–10)  
* **Region** → Southwest / Southeast / Northwest / Northeast  

---

## ⚙️ How It Works
* User enters input values  
* Data is preprocessed:
  * Encoding categorical variables  
  * Feature scaling using StandardScaler  
* Model predicts log-transformed insurance cost  
* Output is converted using exponential function  
* Final predicted price is displayed  

---

## 🛠️ Installation & Setup

### 1️⃣ Clone Repository
```bash
git clone <your-repo-link>
cd <your-project-folder>
```

### 2️⃣ Create Virtual Environment (Windows PowerShell)
```powershell
python -m venv myenv
myenv\Scripts\activate
```

### 3️⃣ Install Dependencies
```bash
pip install streamlit scikit-learn pandas seaborn numpy
```

### 4️⃣ Run Application
```bash
streamlit run app.py
```

---

## 📁 Project Structure
```
├── app.py                 # Main Streamlit app
├── gb_model.pkl          # Trained ML model
├── README.md
|___requirements.txt           # Project documentation
```

---

## 🔮 Model Details
* Algorithm Used: Gradient Boosting (GB Model)  
* Model loaded using Pickle  
* Output is log-transformed and reversed using exponential  

---

## 📌 Sample Prediction Flow
* Input: Age = 25, BMI = 28, Smoker = No  
* Model processes features  
* Output: Estimated insurance cost 💰  

---

## ⚠️ Notes
* Ensure `gb_model.pkl` is present in the project directory  
* Do not refit scaler during prediction in real-world deployment  
* Model accuracy depends on training data  

---

## 💡 Future Improvements
* Add model accuracy metrics  
* Improve UI design  
* Deploy using Docker  
* Add more features (income, lifestyle, etc.)  

---

## 👨‍💻 Author
* Developed as part of Machine Learning practice project  

---

## ⭐ If you like this project
* Give it a star ⭐  
* Share with others 🚀  
