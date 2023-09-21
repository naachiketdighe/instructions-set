# Creating a Flask Application in Python

In this guide, we will walk through the process of creating a basic [Flask](https://flask.palletsprojects.com/en/2.3.x/) application in Python. Flask is a micro web framework, that we can import as a Python module to develop web applications easily.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3c/Flask_logo.svg/1200px-Flask_logo.svg.png)

## Introduction

Python Flask is a powerful and lightweight web framework that allows developers to create web applications with ease. Whether you're a seasoned developer or just starting your journey in web development, Flask offers a straightforward and flexible way to build web applications in Python. Flask allows developers to seamlessly integrate Python with HTML, CSS, and JavaScript for web development. 

In this comprehensive guide, we will walk you through the essential steps and concepts required to get started with Flask. From setting up a development environment to building your first web application, you'll gain a solid understanding of how Flask works and how to leverage its features to create web applications tailored to your needs.

By the end of this tutorial, you'll be equipped with the knowledge and skills to embark on your web development projects using Python Flask. So, let's dive in and explore the world of web development with Flask

## Terms

[Pip](https://pypi.org/project/pip/): Pip is like a magic tool for your computer that helps you easily find and install new programs or pieces of software. It's kind of like a digital shopping assistant for your computer. When you want to add a new program or feature to your computer, you can tell pip what you want, and it will go out and find it for you on the internet. Then, it brings it back and sets it up on your computer so you can use it without any hassle. So, in simple terms, pip is like your computer's helpful friend that brings you cool stuff from the internet and helps you set it up. We will be using pip to install the various libraries required in Python.

[Bash](https://medium.com/@krish.raghuram/terminal-shell-and-bash-3e76218c8865): Bash is a command-line shell, which means it's a program that interprets and executes commands entered by the user. Bash is like the conductor of an orchestra for your computer. It's a special program that lets you talk to your computer and give it instructions by typing text commands. Instead of using a mouse and clicking on icons, with Bash, you type what you want your computer to do, and it listens and does it. It's a bit like having a conversation with your computer in a language it understands. So, think of Bash as your computer's language interpreter, allowing you to tell it what you need it to do, whether it's opening files, organizing folders, or running other programs.

[HTML](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics) provides the structure of a webpage.
[CSS](https://developer.mozilla.org/en-US/docs/Web/CSS) enhances the style and appearance of the webpage.
[JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) adds interactive behavior and functionality to the webpage.

Together, these technologies work harmoniously to create the websites and web applications you use every day on the internet.

## Prerequisites

Before you begin, please make sure you have the following installed:

- Python (3. x recommended)
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
![Installing Python Flask](https://i.ibb.co/k62BB92/Screen-Shot-2023-09-21-at-11-30-00-AM.png)
## Step 2: Create a new directory for the Flask application

Open up the terminal or Bash on your machine

```bash
mkdir Flask_app

cd Flask_app
```
![](https://i.ibb.co/SwD461W/Screen-Shot-2023-09-21-at-11-41-15-AM.png)
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

## Conclusion

By going to a browser of your choice, type in http://127.0.0.1:5000.

![](https://i.ibb.co/GpKdNHJ/Screen-Shot-2023-09-21-at-12-36-19-PM.png)

Thus, you can see the changes made to your website by adding more lines of code, or changing the existing code!

Thus, in this tutorial, we learnt to:
- install Flask
- Creating a Flask App
- using HTML with Flask
- Adding HTML code to your Flask app
- Using a development server to see the changes to your website



