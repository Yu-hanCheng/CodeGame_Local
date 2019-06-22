# Environment settings
1. To install python3, please refer to [here](https://realpython.com/installing-python/) 
2. `pip3 install virtualenv` or refer to [here](https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments)
3. `virtualenv venv` build a virtual environment

# Install Local Test Server
1. `git clone https://github.com/Yu-hanCheng/CodeGame_Local.git`
2. `cd CodeGame_Local`
1. `source ./venv/bin/activate`( `cd venv\Scripts;activate` on Windows )
3. `pip install --upgrade pip`
4. `pip install -r requirement.txt` (scikit-learn==0.20.0, scipy==1.2.1)
6. `export FLASK_APP=localapp.py`( `set FLASK_APP=localapp.py` on Windows )
5. `flask run -p 5500` and Running on http://127.0.0.1:5000/


# About ML code 
1. Training data can be log of rank_list or your test result
2. Example code
```
def run():
    global paddle_vel,paddle_pos,ball_pos,move_unit
    paddle_vel=0
    ballarray=np.array(ball_pos[-1])[:, np.newaxis]
    padarray=np.array(paddle_pos)
    
    x_input=np.vstack([ballarray, padarray]).T
    paddle_vel=int(load_model.predict(x_input)[0])
```

PS. If terminal print out "upload_code", but it has not print the code data for 10 secs, it may indicate that the network is not well. Please check it.