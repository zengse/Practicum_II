
MSDS696_C70 Data Science Practicum II
=======

Data anlysis - Reddit/r/datascience 
=======
:Info: reddit data analysis on 'datascience' topic.And Reddit is a community platform that a millions of users posts,comment and share media contents across the word.The project is a sentiment analysis on posts and comments of users that is taken for a year span
:Author: Dawit Fana ( Gedibe previously)

About
=====

The PyMongo d .

Issues / Questions / Feedback
=============================

Any issues 

Installation
============

If no mongodb instace installed , please follow the steps for installation from mongodb ()
For those who has macos as i do I would suggest using Homebrew. 
Please open up the MacOs command line tool and paste the following command to setup MongoDB on MacOS.

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

Once you entered the given above command, your MacOS terminal will start some process. Those processes are nothing but related to creating some folder in your local machine where all the Homebrew related settings are kept.

After finishing the installation process, check your Homebrew dependencies.


brew update

Hit the below commands to install MongoDB

brew install mongodb-community

After MongoDB successfully installed in your machine, then create a folder to store MongoDB data using given below command


sudo mkdir -p /data/db

Use the given below command to assign the proper permission to MongoDB data folder.

sudo chown -R `id -un` /data/db.

Dependencies
============
pip install requests
pip install json
pip install bokeh
pip install pymongo  
pip install pandas  
pip install numpy
pip install sklearn

Direction 
===========
Once mongodb is installed and data base will be created and populated on fly from the jupyter notebook executables.
Alternatively , you can create a database and collection from a  sample data. This will save you a loading time of a year old comments and texts from Reddit.
Here is the steps to do the alternative data load.

-- start mongodb deamon 
mongod
-- on another tab , start mongo
mongo
-- create a database and a collection to insert sample_data.json
use Practicum_II
db.insertMany(sample_data.json)
