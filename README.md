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

![Opening a new terminal](https://i.ibb.co/bHyB2vS/Screen-Shot-2023-09-11-at-11-56-51-AM.png)

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
from flask import Flask, render_template

# Create a Flask application instance
app = Flask(__name__)

# Define a route and a function to handle the request
@app.route('/')
def hello():
    return render_template(index.html)

# Run the application if this script is executed
if __name__ == '__main__':
    app.run()
```

## Step 5: Create an HTML file

In VSC, on the left-hand side, navigate to the parent folder and right-click to add another folder inside Flask_app

Name this folder Templates(this is important, for Flask to identify your HTML file)

Add a file to the Templates folder, name it index.html, and add the following code:

```HTML
<!DOCTYPE html>
<!--[if lt IE 7]>      <html class="no-js lt-ie9 lt-ie8 lt-ie7"> <![endif]-->
<!--[if IE 7]>         <html class="no-js lt-ie9 lt-ie8"> <![endif]-->
<!--[if IE 8]>         <html class="no-js lt-ie9"> <![endif]-->
<!--[if gt IE 8]>      <html class="no-js"> <!--<![endif]-->
<html>
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <title></title>
        <meta name="description" content="">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <link rel="stylesheet" href="">
    </head>
    <body>
        <!--[if lt IE 7]>
            <p class="browsehappy">You are using an <strong>outdated</strong> browser. Please <a href="#">upgrade your browser</a> to improve your experience.</p>
        <![endif]-->
        
        <script src="" async defer></script>
    </body>
</html>
```

## Step 6: Run your Flask App

In the terminal of VSC, type in the following command:
```python
python app.py
```




