# Yelp Challenge

## Questions for the Yelp Dataset
Yelp is a website that gives recommendations for restaurants and businesses. The provided dataset contains informations about those businesses as well
as information about the persons, who reviewed these.

The files of this repository investigate the dataset based on the following questions:<br>
	1. Does the region have influence on a business? (Investigation_1.ipynp)<br>
	2. What features make a business successful? How are / Are features correlating with the rating of a business? (Investigation_2.ipynp)<br>
	3. What makes a review positiv? How can the sentiment of a review be predicted? (Investigation_3.ipynp)

## Archive Contents
* Data
	- yelp_dataset
		- business.json
		- checkin.json
		- photo.json
		- review.json
		- tip.json
		- user.json
* Docker
	- Dockerfile.Dockerfile <br/> *Dockerfile to create a suitable docker container.*
* Models
	- Investigation_2
		- model_gradient_boosting.pkl <br/> *GradientBoosting Model*
	- Investigation_3
		- Placeholder for the saved models of Investigation_3.ipynp
* Notebooks
	- Investigation_1.ipynp  <br/> *Clustering of businesses*
	- Investigation_2.ipynp  <br/> *Classification of star ratings*
	- Investigation_3.ipynp  <br/> *Sentiment analysis of reviews*

## Data
The original train- and testdata can be downloaded from Yelp.

Link to the data:https://www.yelp.com/dataset/challenge

Information: The datasets have to be stored in the data folder.

### Docker
To execute a Jupyter Notebook inside a docker container, follow the next steps:

* Step 1: Change inside the Docker Terminal to the here downloaded Docker folder
* Step 2: Build the Docker container via `$ docker build -t tfnbe .`
* Step 3: Run Jupyter inside docker via `$ docker run -p 8888:8888 -v ~/my/notebooks:/home/jovyan tfnbe`. Please change `~/my/notebooks` to the direction, where this repository is stored.

## Licence
This code is submitted under [MIT license](https://opensource.org/licenses/MIT).
