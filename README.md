# Disaster-Response-Pipeline


## Table of Contents
     Summary of the project
     File Descriptions
     Insturctions
     
### Summary of the project
The project to classify the messages during nature disasters. By analyzing real messages sent during natural disasters (Data provided by Appen) and using machine learning techiniques to create a multi-output supervised learning model to categorize the messages, the result is visually presented on a web app.

### File Descriptions

  - README.md: read me file
  - ETL Pipeline Preparation.ipynb: contains ETL pipeline preparation code
  - ML Pipeline Preparation.ipynb: contains ML pipeline preparation code
  - workspace
	- app
		- run.py: flask file to run the app
	- templates
		- master.html: main page of the web application 
		- go.html: result web page
	- data
		- disaster_categories.csv: categories dataset
		- disaster_messages.csv: messages dataset
		- DisasterResponse.db: disaster response database
		- process_data.py: ETL process
	- models
		- train_classifier.py: random forecast classification code

### Instructions
   Run the following commands in the project's root directory to set up your database and model.

   > To run ETL pipeline that cleans data and stores in database 
    > python data/process_data.py   
      data/disaster_messages.csv 
      data/disaster_categories.csv 
      data/DisasterResponse.db
      
   > To run ML pipeline that trains classifier and saves 
    > python models/train_classifier.py 
      data/DisasterResponse.db 
      models/classifier.pkl

Run the following command in the app's directory to run your web app. python run.py

Go to http://0.0.0.0:3001/
