# Environment settings
1. To install python3, please refer to [here](https://realpython.com/installing-python/) 
2. `pip3 install virtualenv` or refer to [here](https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments)

# Install Localapp test server
1. `git clone https://github.com/Yu-hanCheng/CodeGame_Local.git`
2. `cd CodeGame_Local`
1. `virtualenv venv`
2. `source ./venv/bin/activate`( `cd venv\Scripts;activate` on Windows )
3. `pip install -r requirement.txt`
4. `export FLASK_APP=localapp.py`
5. `flask db init`
6. `flask db migrate`
7. `flask db upgrade`
8. `flask run` and Running on http://127.0.0.1:5000/
