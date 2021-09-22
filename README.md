# Task-Master

This is a Code Institute Mini Project, the purpose of this project is to put together all the things I have learnt in the **Backend Development** module and will prepare me for my 3rd Milestone project.

## About the project - Task Manager
* It will be built using Flask, MongoDB, and a frontend framework called Materialize.
* It will make CRUD calls, to a Mongo database.
* This will be done in the context of a Flask application.
* With HTML-based user interfaces.

### The `env.py` doc

To create the flask app you need to set up the environment, as the setup contains sensitive info the env.py has been added to `.gitignore`. An example of the code can be seen below with the sensitive data removed.

```
import os

os.environ.setdefault("IP", "0.0.0.0")
os.environ.setdefault("PORT", "5000")
os.environ.setdefault("SECRET_KEY", "<YOUR_SECRET_KEY_HERE>")
os.environ.setdefault("MONGO_URI", "<YOUR_MONGOU_URI_HERE>")
os.environ.setdefault("MONGO_DBNAME", "<YOUR_DBNAME_HERE>")
```

### Deploying to Heroku

To prepare the app for deployment to Heroku I have created a `requirements.txt` file and a `Prockfile`. I did this using the following commands in the terminal:

```
pip3 freeze --local > requirements.txt
```
```
echo web: python app.py > Procfile
```