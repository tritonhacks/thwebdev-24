---
layout: default
title: Getting Started
has_children: false
parent: An Example
permalink: /Example/Getting Started
nav_order: 1
---

# Getting Started
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

{: .note }
> By [Kevin](https://www.linkedin.com/in/kevin-shin-373183188/)

{: .caution}
This documentation is only for Windows.

## Setting up Python in Visual Studio Code
If your computer doesn't have [Visual Studio Code](https://code.visualstudio.com/), install it and follow these steps. In the installation process of Visual Studio Code, don't change anything and press next until it is installed.

Once it is installed, it will look like this.
![Visual Studio Code Welcome Page](../source/assets/images/vsc_welcome_page.png)

Head over to the [Python Website](https://www.python.org/downloads/) and download the latest version.
Once you get this pop up, make sure to check the second box.

![Python Install](../source/assets/images/python_install.png)

After you've installed Python, you have to set your interpreter so that it uses the installed Python. To do so, press ``` CTRL + SHIFT + P ``` inside of your visual studio code and type Python: Select Interpreter and press enter. You should see an option to select the interpreter you just installed.

![Python Interpreter](add image here later)

You've just finished setting up your environment!
## Dependencies
You won't be able to install any of these dependencies if you do not have your Python set up.
{: .attention}

In order to access the framework we'll be using, you must install the libraries first. To do so, go into your Visual Studio Code and make sure that your interpreter is set as the one you just installed. Press ``` Ctrl + Shift + P ``` and type in Terminal: Create New Terminal. Inside of this terminal, type these two commands separately.
```bash
pip install fastapi
```
```bash
pip install uvicorn
```

Once these are installed, you are all set up to start creating your website.

[Previous: Example](Example){: .float-left .v-align-text-top}
[Next: Design Process](Example/Design Process){: .float-right .v-align-text-top}