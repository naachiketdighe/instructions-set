# Creating a Flask Application in Python

In this guide, we will walk through the process of creating a basic [Flask](https://flask.palletsprojects.com/en/2.3.x/) application in Python. Flask is a micro web framework, that we can import as a Python module to develop web applications easily.

## Prerequisites

Before you begin, please make sure you have the following installed:

- Python (3.x recommended)
- Pip (Python package manager)
- Basic knowledge of web development(HTML, CSS and JS)
- Visual Studio Code(VSC) (recommended, but please feel free to use another IDE)

## Step 1: Install Flask

You can install Flask using pip. In VSC, under Terminal, select open new terminal, as shown below

![Opening a new terminal](https://ibb.co/vsrPQd7)

Inside the terminal, make sure you have pip installed, and then install Flask
```python
pip --version

pip install Flask
```

## Step 2: Create a new directory for the Flask application

Open up the terminal or Bash on your machine

```bash
mkdir Flask_app

cd Flask_app
```

## Step 3: Create a new python file

Open up VSC on your machine, and then click on Open new folder and then navigate to the folder you just created

Under File, select New File and then select Create a new File and name it app.py

## Step 4: Create a Flask App

In your app.py, add the following code below:

```python
from flask import Flask

# Create a Flask application instance
app = Flask(__name__)

# Define a route and a function to handle the request
@app.route('/')
def hello():
    return 'Hello, World!'

# Run the application if this script is executed
if __name__ == '__main__':
    app.run()
```






