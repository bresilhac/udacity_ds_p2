# Disaster Response Pipeline Project
### Summary:
This is a web application written in python to automatically classify text messages into different categories of disaster management. Furthermore, two visualizations from the data set are available as examples. This application will help the disaster victims to receive prompt medical aid and speedy recovery from the effects of the disasters. In this way the application will benefit those whose responsibility is to help those in need during a time of natural disaster.

The project consists of 3 areas. 
1. ETL pipeline (process_data.py) to cleans data and store data for further processing
2. ML pipeline (train_classifier.py) to train and save a classifier model
3. Flask web app (run.py) for interactive classification based on trained model of arbitary text data and visualisations of some data

### Requirements:
You will need following python packages in order to execute the project: 
* flask
* plotly
* sqlalchemy
* pandas
* numpy
* sklearn
* nltk

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

### xseibel deserves total credit for the inspiration of this project.
