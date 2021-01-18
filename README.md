# Objective
As the name says, it is simply scrapping all the national assembly sessions.
The data is taken on the https://www.nosdeputes.fr/ website, which is not the official national assembly website, but is an anonymous citizen-produced website that gives a cleaner and more insightful version of the original sessions. They make it way easier to scrap while producing relevant data on their own (ex: tags, a deputy database, etc.)

# Scrapping national assembly notebook
It is getting all the assembly session retranscriptions on multiple JSON files.

# Joining national assembly sessions - data processing
Merges the different JSON files on a csv to have all the interventions per speaker (not appropriate to treat these data per sessions, as the information is lost in the process).
First steps of data processing, mostly by eliminating usual and custom stop words.

# Scrapping deputy list notebook
Used to get all deputies metadatas on a single csv file. The given csv still need a small post-data cleaning, cleaning null rows that are the ones standing for the most inactive deputies. This will be fixed on later updates.

Of course, the output from these two notebooks have been made to be joinable on the "nom" (name) column.

# Data processing and topic modelling
As implied in the name, this notebook contains some data processing, a failed topic modelling attempt, and a working topic modelling algorithm.
