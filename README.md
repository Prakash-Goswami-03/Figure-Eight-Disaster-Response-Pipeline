# Figure-Eight-Disaster-Response-Pipeline
### Disaster Reponse Pipeline for Udacity Data Science nanodegree

This Web app uses Machine Learning to predict the classification of a given typical disaster emergency response text message. For example, if the input is: "My house is burning down", the classification category should be "Fire". This application is useful to identify emergency response services required.

This Flask Web app was developed using Python and SKLearn machine learning libraries for Natural Language Processing (NLP).

### Installation: 
Clone the GitHub repository and use Anaconda distribution of Python 3.6.7.

    $ git clone https://github.com/cristiandatum/DS_Response_Pipeline.git

In addition This will require pip installation of the following:

    $ pip install SQLAlchemy
    $ pip install nltk

The code can be viewed and modified with Spyder Notebooks.

### Data:
1. disaster_messages.csv - Disaster messages are available in this file.
2. disaster_categories.csv- categories of messsages are mentioned in this file.
3. DisasterResponse.db - database file where messages are stored after data processing.


### Instructions:

Run the following commands in the project's root directory to set up your database and model.

To run ETL pipeline that cleans data and stores in database:

    $ python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db

To run ML pipeline that trains classifier and saves model:

    $ python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl

Run the following command: model in the app's directory to run your web app: 

    $ python app/run.py
    
 Go to: `http://0.0.0.0:3001/`




### Acknowledgments:
The .csv files containing data from real disaster response messages was provided by Udacity from Figure Eight.
The started code was provided by Udacity.
