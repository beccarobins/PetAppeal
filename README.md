# PetAppeal

Welcome to the PetAppeal repo! This repo contains codes that allow you to easily query, clean, and model data gathered from the Petfinder database. The ultimate aim of the PetAppeal project is to determine the factors leading to pet adoptions and help promote pet adoption in the United States. 

## Petfinder API
The Petfinder API lets users easily query the Petfinder database for animal shelter information, individual pet information, and breed information. A total of 10,000 requests can be made per day and a maximum of 1,000 records can be returned per request. To get started, you will need to request an API (https://www.petfinder.com/developers/api-docs). A csv of all shelters listed in the Petfinder database between November 22 and November 26, 2017 has been provided.

## No Kill Network
The No Kill Network is an organization that promotes no kill animal shelters across the United States. A list of the no kill shelters in the U.S. was scraped from the No Kill Network website (https://www.nokillnetwork.org/) to elucidate the exact status of the individual animals, as both adopted and euthanized animals are listed as 'Removed' in the Petfinder database. The list of no kill shelters is provided in this repository; however, there is lots of missing information. Please feel free to comment if you have information that can update and complete this list.

## Workflow
The general workflow for PetAppeal is 1) query to find animal shelters, 2) query to find pets, 3) clean the data, 4) visualize, and 5) model. Provided herein is a workflow that queries for pets using the No Kill Network list as a filter, which is ultimately used to predict adoption status, i.e., whether the animal is still in the shelter or has been adopted using a random forest classification model. The code is easily modifiable for use with other models and for other questions.

### 1) 
