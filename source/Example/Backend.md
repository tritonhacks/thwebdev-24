---
layout: default
title: Creating the Backend
has_children: false
parent: An Example
permalink: /Example/Backend
nav_order: 4
---

# Creating our Backend
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

{: .note }
> By [name](github or linkedin)

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

[Previous: Frontend](Frontend){: .float-left .v-align-text-top}
[Next: Building our Website](Website){: .float-right .v-align-text-top}
