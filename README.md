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
