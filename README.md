# Smishing Detection

## Tech Stack
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) 
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) 
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white) 
![Scipy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white) 
![Streamlit](https://img.shields.io/badge/Streamlit-%23FE4B4B.svg?style=for-the-badge&logo=streamlit&logoColor=white)

## Overview
This project aims to classify text messages to detect potential smishing (SMS phishing) attacks. Using machine learning, the project provides a classifier that can differentiate between legitimate messages and smishing attempts, helping to prevent scams.

The classification model is deployed using a Streamlit app, allowing users to input text messages and get real-time classification results.

## Files
- **app.py**: Streamlit application code. This file loads the trained model and vectorizer and uses them to classify input messages as smishing or legitimate.
- **model.pkl**: Trained classification model for detecting smishing messages.
- **vectorizer.pkl**: Pre-trained vectorizer model used to transform input text data for classification.
- **nltk.txt**: File specifying NLTK dependencies (e.g., stop words) needed for text preprocessing.
- **requirements.txt**: List of dependencies required to run the project, including Streamlit and other libraries.

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/SudarshanC00/Smishing.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Smishing
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Download required NLTK data:
   ```bash
   python -m nltk.downloader -d /usr/local/share/nltk_data -r nltk.txt
   ```

## Usage
1. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```
2. Open the provided local URL in your browser.
3. Enter a text message to classify it as either legitimate or smishing.

## Model Details
- The model and vectorizer were pre-trained to accurately classify smishing messages.
- Both the model and vectorizer files (`model.pkl` and `vectorizer.pkl`) are loaded in `app.py` to make predictions.

## License
This project is licensed under the MIT License.
