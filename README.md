Mushroom Classifier
===================================

Mashroom classifer is flask based web application that is powered by machine learning model. The model is trained on [Kagel](https://www.kaggle.com/uciml/mushroom-classification) dataset with set of features and lebles for mushroom eatibility e.g. edible "e" and poisnous "p". 

## Training Classifier
* Classifier is trained using "mashrooms.csv" dataset under ./data/mashrooms.csv
* Training script can be found under ./jupyter_notebook/Train_Mushroom_Classifier.ipynb
* Following algorithms were used to train three different models
	- KNearestNeighbour
	- DecisionTrees
	- GradientBoosting (best)
* Models are stored under ./model directory

## Flask based web application
* Fornt end is a single page web form that lets user choos different features (total 22) of mushrooms
* Clicking button "Predict eatbility" posts JSON request to the server and gets response with two classes ('e', 'p')
* After running "app.py" wep app can be accessed at http://127.0.0.1:5000

## Dependencies
* All the python dependencies are listed in "requirement.txt" file and are as following:

	-	Click==7.0
	-	cycler==0.10.0
	-	Flask==1.0.3
	-	itsdangerous==1.1.0
	-	Jinja2==2.10.1
	-	kiwisolver==1.1.0
	-	MarkupSafe==1.1.1
	-	matplotlib==3.1.0
	-	numpy==1.16.4
	-	pandas==0.24.2
	-	pyparsing==2.4.0
	-	python-dateutil==2.8.0
	-	pytz==2019.1
	-	scikit-learn==0.19.1
	-	scipy==1.3.0
	-	six==1.12.0
	-	Werkzeug==0.15.4
