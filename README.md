# Disaster Response Pipeline

## Build Pipelines to Classify Messages with Figure Eight

This project is a part of my Udacitiy Nanodegree which Aims to builds a data pipeline to prepare message data from major natural disasters around the world. I build an ETL and RandomForest pipeline to categorize emergency messages based on the needs communicated by the sender.

## Main Steps

1. Clean data by Natural Language Processing (Normalized, tokenized and lemmatized the text messages)
2. Built up pipelines to train Random forest with grid search; Applied TF-IDF to assign the weights to words in the message
3. Use Random Forest in the final model and test results in the website

Data Source: Figure Eight, San Francisco, CA

## Install the Requirements
If you are running this in your local environment, run conda install --file requirements.txt

Or pip install -r requirements.txt to install the required python module dependencies

## Instructions

Run the following commands in the project's root directory to set up database and model.

•	To run ETL pipeline that cleans data and stores in database -
  python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/Disaster.db

•	To run ML pipeline that trains classifier and saves -
  python models/train_classifier.py data/Disaster.db models/classifier.pkl

## Running the Web App from the Project Workspace IDE

Step 1: Type in the command line: python run.py

Step 2: Open another Terminal Window, Type: env|grep WORK

Step 3: In a new web browser window, type in the following: https://SPACEID-3001.SPACEDOMAIN where SPACEID & SPACEDOMAIN are shown in step 2.

## Environment and Libraries Used

Environment - Jupyer Notebook and Python IDE (Atom)

1. NumPy
2. Pandas
3. Scikit-Learn
4. Plotly
5. SQLAlchemy
5. Flask

## Acknowledgement

I would like to Thank Udacity for providing with this Interesting Project and Future Eight or providing the Data and Assistance.
