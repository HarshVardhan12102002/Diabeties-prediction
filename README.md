
# Diabetes Prediction ML Project

This project aims to predict whether a patient has diabetes based on certain diagnostic measurements. The model is built using machine learning techniques and deployed as a web application for user interaction.

## Project Structure

```bash
diabetes_prediction/
├── diabetes.csv                     # Dataset used for model training and testing
├── Diabetes_Prediction_mlModel.ipynb # Jupyter notebook for building and training the ML model
├── predictive_system.py              # Python script for prediction using the trained model
├── diabetes_prediction_web_app.py    # Python script for the web application interface (using Flask)
├── trained_model.sav                 # Serialized trained model for reuse in predictions
├── requirements.txt                  # Python dependencies for running the project
└── README.md                         # Project documentation
```

### 1. **diabetes.csv**
   - This is the dataset used for training and testing the machine learning model. The dataset contains several medical attributes (e.g., glucose level, BMI, age) used to predict whether the patient is diabetic or not.

### 2. **Diabetes_Prediction_mlModel.ipynb**
   - A Jupyter Notebook where the diabetes prediction model is built and trained. It includes data preprocessing, feature selection, model building, and evaluation steps. The notebook uses various machine learning techniques to develop an accurate prediction model.

### 3. **predictive_system.py**
   - A Python script that loads the trained model (`trained_model.sav`) and allows users to input new data to predict whether a person is diabetic. It acts as a predictive system by utilizing the saved machine learning model for real-time predictions.

### 4. **diabetes_prediction_web_app.py**
   - This script implements the web-based user interface for the diabetes prediction system using Flask. Users can input values such as glucose levels, BMI, age, etc., and get real-time predictions of whether they are at risk for diabetes.

### 5. **trained_model.sav**
   - This file contains the saved model after training. It is a serialized version of the trained machine learning model and can be loaded in `predictive_system.py` or `diabetes_prediction_web_app.py` to make predictions without retraining the model.

### 6. **requirements.txt**
   - This file lists the required Python packages and dependencies to run the project. Install them by running:

     ```bash
     pip install -r requirements.txt
     ```

---

## How to Run the Project

### Prerequisites:
- Python 3.7+
- Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

### Step 1: Train the Model (optional)
   If you want to train the model from scratch, open `Diabetes_Prediction_mlModel.ipynb` in Jupyter Notebook and run all the cells. This will train the model and save it as `trained_model.sav`.

### Step 2: Run the Web Application
   To launch the web application and make predictions:
   
   ```bash
   python diabetes_prediction_web_app.py
   ```

   The app will be hosted locally, and you can access it via your browser at `http://127.0.0.1:5000/`. Enter the necessary patient details, and the system will predict whether the patient is diabetic or not.

### Step 3: Use the Predictive System Script
   If you prefer using a command-line script to make predictions, run:

   ```bash
   python predictive_system.py
   ```

   The script will prompt you to input the required medical attributes, and it will return a prediction based on the trained model.

---

## Dataset

The dataset used in this project is publicly available and contains medical diagnostic measurements for diabetes prediction, such as:
- Pregnancies
- Glucose level
- Blood pressure
- Skin thickness
- Insulin level
- BMI (Body Mass Index)
- Diabetes Pedigree Function
- Age

---

## Technologies Used
- **Python**: Core programming language for development.
- **Flask**: Used to develop the web application.
- **scikit-learn**: For model building and evaluation.
- **pandas**: For data manipulation and analysis.
- **Jupyter Notebook**: For building and training the machine learning model.

---

## Contributing
Feel free to contribute to this project by submitting issues or pull requests.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

### Contact
For any queries or issues, feel free to reach out at [your-email@example.com].
