# Flask-Workshop-FOSS

## Installation

### Step 1: Set up a virtual environment

##### Check your Python version

```python
python --version
```

#### Make a New Folder for the Project

```python
mkdir flask_project
```

```python
cd flask_project
```

#### Install the virtual environment

```python
pip3 install virtualenv
```
```python
virtualenv env
```

### Step 2: Activate the env 

For Mac/Linux
```python
source env/bin/activate 
```

For Windows
```python
.\env\Scripts\activate
```
### Step 3: Install the requirements

```python
pip3 install flask
```

### Step 4: Create a new file called 'app.py'

### Step 5: Adding code (Setting Up) inside 'app.py'

```python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    return "Hello, World!"

if __name__ == "__main__":
    app.run(debug=True)
```

### Step 6: Run the environment

```python
python3 app.py
```

### Step 7: Stopping the environment

Control + C

### Extra Info

If your trying to create an index.html file and you want to link it to the app.py

Create an index.html file and then change app.py to:

```python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    return render_template('index.html')

if __name__ == "__main__":
    app.run(debug=True)
```



