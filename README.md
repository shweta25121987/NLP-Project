This project aims to predict whether a given tweet is related to a disaster or not using machine learning. The trained model is then deployed as a web application using Flask, allowing users to input tweets and receive real-time predictions.

Prerequisites
Before running the project, ensure you have the following dependencies installed:

Python (version 3.6 or higher) pip package manager Flask (install via pip install Flask) scikit-learn (install via pip install scikit-learn) pandas (install via pip install pandas) numpy (install via pip install numpy)

Project Structure
The project is structured as follows:

├── app/

│ ├── static/

│ │ └── styles.css

│ ├── templates/

│ │ └── index.html

│ ├── app.py

│ └── model.pkl

├── data/

│ └── disaster_tweets.csv

├── notebooks/

│ └── train_model.ipynb

└── README.md

app/: Contains the Flask web application.
static/: CSS styles for the web interface.
templates/: HTML templates for the web pages.
app.py: Flask application script.
model.pkl: Trained machine learning model saved as a pickle file.
data/: Contains the dataset used for training the model (disaster_tweets.csv).
notebooks/: Contains Jupyter notebooks used for training the model (train_model.ipynb).
README.md: This README file.
Training the Model
To train the model, follow these steps:

Open and run the Jupyter notebook train_model.ipynb located in the notebooks/ directory. The notebook will load the dataset (data/disaster_tweets.csv), preprocess the data, train the model, and save it as app/model.pkl.

Running the Web App
To run the web application, follow these steps:

Navigate to the app/ directory. Run the Flask application using the following command: python app.py

Once the application is running, open a web browser and go to http://localhost:5000 to access the web interface.

Using the Web Interface
In the input field, enter the tweet text that you want to classify. Click the "Predict" button. The predicted class (disaster or not) will be displayed on the web page. Contributing If you would like to contribute to this project, feel free to submit a pull request.
