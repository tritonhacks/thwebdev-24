---
layout: default
title: Creating the Backend
nav_order: 3
permalink: /Example/Backend
parent: An Example
has_children: false
---

# Creating our Backend
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

### <img src="../source/assets/images/fastapi-1.svg" alt="FastAPI Logo" width="15" height="15"> FastAPI
For our Web Development Starter Kit, we'll be utilizing FastAPI, an essential toolkit for those creating websites and web applications. Consider FastAPI as a collection of foundational tools that developers employ to build and manage the unseen components of websites or apps. These components are crucial for functions like securely transmitting your data during sign-ups or log-ins.

While there are other frameworks like Flask, Django, and Tornado, each serving distinct purposes, FastAPI stands out for its ease of use and robust built-in features. This means you can achieve more with less coding effort, making it an excellent choice for both quick website deployment and for those new to web development, thanks to its gentle learning curve.

Complete [Getting Started](Getting Started) before doing this.
{: .caution}

#### **Working with FastAPI**
Create an app.py file at the root level of your project folder. Inside of it, write these lines of code.
```python
from fastapi import FastAPI
from fastapi.staticfiles import StaticFiles       # Used for making static resources available to server
from fastapi.templating import Jinja2Templates # Used for templatizied HTML
import uvicorn

# Here, you're creating an instance of FastAPI. 
# This is like starting up your FastAPI toolkit and getting it ready to use. 
# We call this instance app, and it's what you'll use to create different parts of your web application.
app = FastAPI() 

# Specify where the static files are located. This is the name of your folder.
static_files = StaticFiles(directory='public') 
views = Jinja2Templates(directory="public/views")

# Mount the static files directory to /public, this is where your other files will access the sources.
app.mount('/public', static_files, name='public')

# We modulate the different kinds of files so it's easier for us to navigate them
app.mount("/imgs", StaticFiles(directory="public/imgs"), name="imgs")
app.mount("/css", StaticFiles(directory="public/css"), name="css")
app.mount("/js", StaticFiles(directory="public/js"), name="js")

if __name__ == "__main__":
    # We can specify what ports to run, and you can change this.
    # You would access this at 127.0.0.`:8007 or localhost:8007
    # reload = True allows us to make changes to our code without constantly rerunning the code.
    uvicorn.run("FileName:app", host="127.0.0.1", port=8007, reload=True)
```

We're then going to add these routes.
```py
@app.get("")

@app.post("")

@app.put("")

@app.delete("")
```

### Getting Started With FastAPI 

```py
from fastapi import FastAPI

app = FastAPI()
```

First we have to import FastAPI to our code. When we import FastAPI we are adding the FastAPI class to our code which allows us to use the functionality of FastAPI. 

```py
from fastapi import FastAPI
```

Then we create a FastAPI instance. Here our ```app``` variable will be an instance of the class FastAPI which will be our main point of interaction for all of our API. API stands for Application Programming Interface.  

```py
app = FastAPI()
```
---

```py
from fastapi import FastAPI
from fastapi.staticfiles import StaticFiles

app = FastAPI()
```
Next we have to import the StaticFiles class from FastAPI to allow us to serve our static files like JavaScript, css, and images from a directory in our file system to our browswer. 

```py
from fastapi.staticfiles import StaticFiles
```

Then we mount a ```StaticFiles()``` instance in a specific path. When we refer to mounting, it means adding a complete "independent" application in  a specific path, that then takes care of handling all the sub-paths.

Here is a breakdown of the "app.mount()":

```app.mount("/imgs", StaticFiles(directory="public/imgs"), name="imgs")```

The first ```"/imgs"``` refers to the sub-path this "sub-application" will be "mounted" on. So, any path that starts with ```"/imgs"``` will be handled by it.

The ```directory="public/imgs"``` refers to the name of the directory that contains your static files.

The ```name="imgs"``` gives it a name that can be used internally by FastAPI.

```py
from fastapi.staticfiles import StaticFiles

app.mount("/imgs", StaticFiles(directory="public/imgs"), name="imgs")
app.mount("/css", StaticFiles(directory="public/css"), name="css")
app.mount("/js", StaticFiles(directory="public/js"), name="js")
```


[Previous: Frontend](Frontend){: .float-left .v-align-text-top}
[Next: Building our Website](Website){: .float-right .v-align-text-top}
