# Disaster Response Pipelines

Different types of disaster response organizations take care of different parts of the disasters and observe messages to understand the needs of the situation. They have the least capacity to filter out messages during a large disaster, so predictive modeling can help classify different messages more efficiently.

The final deliverable is Flask app that classifies input messages and shows visualizations of key statistics of the dataset.

### Files:

#### process_data.py: 

ETL script to clean data into proper format by splitting up categories and making new columns for each as target variables.

#### train_classifier.py: 

Script to tokenize messages from clean data and create new columns through feature engineering. The data with new features are trained with a ML pipeline and pickled.

#### run.py : 

Main file to run Flask app that classifies messages based on the model and shows data visualizations.

### Instructions:

##### Run the following commands in the project's root directory to set up your database and model.

##### Run ETL pipeline that cleans data and stores in database python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/disaster_message_categories.db

##### Run ML pipeline that trains classifier and saves python models/train_classifier.py data/disaster_message_categories.db models/model.py
