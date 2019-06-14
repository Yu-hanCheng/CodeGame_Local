# Environment settings
1. To install python3, please refer to [here](https://realpython.com/installing-python/) 
2. `pip3 install virtualenv` or refer to [here](https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments)
3. `virtualenv venv` build a virtual environment

# Install Localapp test server
1. `git clone https://github.com/Yu-hanCheng/CodeGame_Local.git`
2. `cd CodeGame_Local`
1. `source ./venv/bin/activate`( `cd venv\Scripts;activate` on Windows )
3. `pip install --upgrade pip`
4. `pip install -r requirement.txt`
6. `export FLASK_APP=localapp.py`( `set FLASK_APP=localapp.py` on Windows )
5. `flask run -p 5500` and Running on http://127.0.0.1:5000/
