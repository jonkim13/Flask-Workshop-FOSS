# Flask-Workshop-FOSS

## Table of Contents
- [Installation]
- [Running the App Locally]
- [Project Structure]
- [Example Code]
- [Stopping the App]

## Installation

### Step 1: Set up a virtual environment

```python
python -m venv venv
```

```python
source venv/bin/activate  # For macOS/Linux
```

```python
venv\Scripts\activate     # For Windows
```

### Step 2: Install the required packages

```python
pip install -r requirements.txt
```

### Step 3: Running the App Locally

```python
python app.py
```
### Step 4: Example Code

```python
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def home():
    return render_template('index.html')

if __name__ == '__main__':
    app.run(debug=True)
```
