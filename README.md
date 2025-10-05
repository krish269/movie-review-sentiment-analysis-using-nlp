Movie Review Sentiment Analysis Web App 🎬
This project is a web application that uses Natural Language Processing (NLP) to classify movie reviews as either positive or negative. The machine learning model is trained on the popular IMDB Dataset and is wrapped in an interactive user interface built with Streamlit.

✨ Features
Interactive UI: A clean and user-friendly web interface to enter movie reviews for analysis.

Real-time Predictions: Instantly classifies the sentiment of the text you provide.

Efficient Workflow: The model is trained and saved in a separate script, allowing the web app to load quickly and perform predictions on demand.

Confidence Score: Displays the model's confidence level in its prediction, giving you a better understanding of the result.

🛠️ Technologies Used
Backend: Python

Machine Learning: Scikit-learn (Logistic Regression)

NLP: NLTK (Natural Language Toolkit) for text preprocessing

Web Framework: Streamlit for the interactive UI

Data Manipulation: Pandas

Model Serialization: Joblib

📂 Project Structure
.
├── sentiment_model.pkl    # Saved trained machine learning model
├── tfidf_vectorizer.pkl   # Saved TF-IDF vectorizer
├── IMDB Dataset.csv       # The dataset for training the model
├── app.py                 # The main Streamlit application script
├── download_nltk.py       # Utility script to download NLTK data
├── requirements.txt       # A list of all required Python packages
└── train_model.py         # Script to preprocess data and train the model

🚀 Setup and Installation
Follow these steps to set up and run the project on your local machine.

1. Prerequisites
Python 3.7+

Git

2. Clone the Repository
Open your terminal and clone the repository to your local machine:

git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
cd your-repository-name

3. Create a Virtual Environment
It is highly recommended to use a virtual environment to manage project dependencies.

# Create the virtual environment
python -m venv venv

# Activate it
# On Windows:
venv\Scripts\Activate.ps1
# On macOS/Linux:
source venv/bin/activate

4. Install Dependencies
Install all the required packages using the requirements.txt file.

pip install -r requirements.txt

(Note: If you don't have a requirements.txt file yet, you can create one by running pip freeze > requirements.txt after installing the packages manually.)

5. Download NLTK Data (Run Once)
The text preprocessing functions depend on data packages from NLTK. Run the utility script to download them.

python download_nltk.py

6. Train the Model (Run Once)
You need to train the model on the IMDB Dataset.csv. This will create the sentiment_model.pkl and tfidf_vectorizer.pkl files that the app needs.

python train_model.py

This step will take a few minutes to complete as it processes all 50,000 reviews.

7. Launch the Streamlit App
Once the model is trained, you can start the web application.

streamlit run app.py

Your default web browser will automatically open with the application running.

💡 How to Use
Once the app is running, you will see a title and a text area.

Type or paste any English-language movie review into the text box.

Click the "Analyze Sentiment" button.

The app will display the predicted sentiment (Positive 👍 or Negative 👎) along with the model's confidence percentage.

OUTPUTS
<img width="940" height="817" alt="image" src="https://github.com/user-attachments/assets/6b9afdb1-dfa7-4698-a93d-1e69acfef8e0" />
<img width="608" height="517" alt="image" src="https://github.com/user-attachments/assets/4a9a3c0e-21cf-48ad-9fa1-6a674f91b91d" />




📄 License
This project is licensed under the MIT License. See the LICENSE file for more details.
