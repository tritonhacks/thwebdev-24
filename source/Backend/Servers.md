---
layout: default
title: Servers
has_children: false
parent: Backend
permalink: /Backend/Servers
nav_order: 1
---

# What are Servers? 
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

{: .note }
> By [Noah Terrell](github or linkedin)

### Simple Definition: 💻
{: .no_toc }
A web server is a computer that stores and serves website files to other computers over the internet. It’s kind of like a library that has all of the books (websites) and gives them to people (computers) who want to read them.


**Lets Dig Deeper**

In the context of websites, web servers can refer to the hardware or software, or both of them working together.🔌🔀

## Hardware: ⚙️🔩
On the hardware side, a web server is a computer that stores web server software and a website's component files like pictures, html, css, and javascript files. This web server is also able to exchange data between other devices connected to the web. 

When referring to a computer as a web server, you may think of a computer like your laptop or PC at home. Yes, these are computers that can serve as web servers, as shown in Image 1. Web servers can run on any computing device that is able to run the web server software. They are also commonly run on computers specifically designed to serve the purpose as a server, which are called rack servers. These servers are encased in a large cabinet, as shown in Image 2.

![Image of desktop computer](../source/assets/images/desktop-Image.jpg) 	![Image of server rack](../source/assets/images/server-rack-image.png)

### Resources With  Hardware Analogy <span style="font-size:120%;">💾</span>

One way to think about the hardware of a web server (the computer 🖥️) is to look at it like it's the kitchen of a restaurant 🧑‍🍳. We know that in order for a restaurant to work, it needs kitchen equipment like the stove, sink, oven, etc. Similarly, for a computer to work, it needs hardware resources such as the CPU, RAM, motherboard, storage, etc. Now that we have all of these components working together in the computer, we are ready to use it as our web server. However, we still need the software aspect for our web server to be fully functional. Just like how the kitchen is useless without staff to prepare food 🍜. Let's now look at the software side of the web server. 


## Software: <span style="font-size:150%;">🧠</span> 

Web server software encompasses programs or applications installed on a computer, enabling it to perform the functionality of a web server. This includes responding to requests from web browsers and serving web content over the internet. At its core, a web server includes an HTTP server—a software component that interprets URLs and HTTP, allowing access to hosted files via domain names and delivering website content to users.


**HTTP Explanation: 🖥️➡️🛜⬅️🧑‍💻**

At the most basic level, whenever a web browser needs a file that is hosted on a web server, the browser requests the file via HTTP. When the request reaches the correct (hardware) web server, the (software) HTTP server accepts the request, finds the requested document, and sends it back to the browser, also through HTTP. (If the server doesn't find the requested document, it returns a 404 response instead.)

![Image of HTTP request](../source/assets/images/HTTP-request-image.png)


### Resources With Software Analogy <span style="font-size:150%;">🧑‍🍳➡️🤵⬅️🍽️😎</span> 

These programs handle various tasks that utilize the computer's resources. Some of the computer's components that the web server software uses, for example, are the CPU (Central Processing Unit) to process tasks 🧠, interpret requests, and execute code. It uses the RAM (Random Access Memory) to store data and code that the web server needs to access quickly, including website files 📁 and database information. Additionally, it utilizes the computer's storage 💾 to store things like website files and databases. Lastly, the Network Interface enables communication between the web server and clients (web browsers) over the internet🛜.


Returning to the analogy of the web server as a kitchen, just as a kitchen has equipment that needs to be utilized, the server (computer) has components that we need to use in order to function as a web server. We can think of the software as the restaurant staff and the website files as the food.

When the chefs receive an order and use the stoves to prepare the food, this is similar to how the web servers receive a request and then use resources like the CPU to process the request and look for the website files🔀📁. Then, when the food is ready to be served, the chefs give the server the food to then be delivered to the customer. Similarly, when the web server finds the website files from the storage, it then uses the network interface to deliver the website files to the user🛜.
 

To summarize this analogy comprehensively, including all parts of the web server, we can think of it like this: When a user visits a website, it's like entering a restaurant and placing an order. The web server (kitchen) receives the request, processes it using the web server software (staff), retrieves the necessary website files (food) from storage (kitchen equipment), and serves them back to the user, allowing them to enjoy the content of the website, much like savoring a delicious meal at a restaurant. 🍽️😋

![Image web server kitchen analogy](../source/assets/images/web-server-kitchen-image.jpg)

[Previous: Backend](../Backend){: .float-left .v-align-text-top}
[Next: Databases](Databases){: .float-right .v-align-text-top}
