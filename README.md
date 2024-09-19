# Flask-Workshop-FOSS

## Installation

### Step 1: Set up a virtual environment

##### Check your Python version

```python
python --version
```

#### Make a New Folder for the Project

#### Install the virtual environment

```python
pip3 install virtualenv
```
```python
virtualenv env
```

### Step 2: Activate the env

```python
source env/bin/activate
```
### Step 3: Install the requirements

```python
pip3 install flask
```

### Step 4: Create a new file called 'app.py'

### Step 5: Working inside 'app.py'

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

