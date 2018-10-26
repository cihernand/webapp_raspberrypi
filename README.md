# Designing your own website and running it on a raspberry pi. What cybersecurity tools do you need to consider?
Low cost software and hardware creates the opportunity to bring empowering technology to people with low-budget. In this project I hope the people  learn to install an operating system and the software needed to design a website using a raspberry pi. Prototyped source code to design the website will be tested in advance to be re-used during the session. The structure of the code will be modular and flexible to incorporate people ideas.

We expect that the audience take this exercise as a initial step to think about how to create secure websites and which tools exist to prevent hacks.  After having an introduction to the vulnerabilities of  websites we could discuss how sites with sensitive data protect themselves in the cyberspace.

#Project tools: Python v3, Flask and MYSQL


#Raspberry project \
https://www.raspberrypi.org/

#Flask project \
http://flask.pocoo.org/

#Tutorial to create a webserver with Flask, code explained step by step: \
https://www.youtube.com/watch?v=zRwy8gtgJ1A

#Visit this Github repository to download the code for the Flask application: \
https://github.com/bradtraversy/myflaskapp

#Virtual enviroment explanation \
https://www.youtube.com/watch?v=N5vscPTWKOk

Installation requirements:

#You may need to install the Python and MySQL development headers and libraries like so: \
sudo apt-get install python3-dev \
sudo apt-get install  libmysqlclient-dev  mysql-server 


#Install Virtual Environment \
sudo apt install virtualenv \
Create Virtual Environment \
virtualenv   myapp  -p [insert path to python3] 

#Activate Virtual Environment \
source myapp/bin/activate

#Install Flask and MySQL python modules \
pip install Flask \
pip install mysql-python \
pip install mysqlclient \
pip install flask-mysqldb

#Install Forms and Hashing passwords python modules \
pip install wtforms \
pip install passlib \
pip install --upgrade setuptools \
pip freeze > requirements.txt

#Commands to run the application

#Access MySQL & create the database for the website \
mysql -u [insert username] -p [insert password]

#Run Flask application \
python app.py 

#Open your web-browser with the following URL\
 http://127.0.0.1:5000/ 

#SQL injections tutorial \
https://www.go4expert.com/articles/complete-mysql-injection-newbies-t20438/




