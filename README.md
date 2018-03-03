# flask-boilerplate
A simple scalable flask boilerplate based on Miguel Grinberg's Mega Flask Tutorial

Fork this repository and then clone it to start working on your flask project.

Based on python 3.6.4


**Steps**

1. Create a virtual environment inside the cloned repository and activate it

    [cloned-repo]$ virtualenv --python=python3.6 venv
    [cloned-repo]$ source venv/bin/activate
    
2. Install all the requirements

    (venv)$ pip install -r requirements.txt
    
3. (venv) $ export FLASK_APP=microblog.py
(venv) $ export FLASK_DEBUG=1
(venv) $ flask run
(venv) $ pip install flask-sqlalchemy
(venv) $ pip install flask-migrate

Write all your models inside models.py

Create the migration repository
(venv) $ flask db init

Make your first database migration
(venv) $ flask db migrate

Apply the changes
(venv) $ flask db upgrade

Because this application uses SQLite, the upgrade command will detect that a database does not exist and will create it (you will notice a file named app.db is added after this command finishes, that is the SQLite database). When working with database servers such as MySQL and PostgreSQL, you have to create the database in the database server before running upgrade.

