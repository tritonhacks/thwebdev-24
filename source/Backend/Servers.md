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

### Simple Definition:
A web server is a computer that stores and serves website files to other computers over the internet. It’s kind of like a library that has all of the books (websites) and gives them to people (computers) who want to read them.


### Lets Dig Deeper: 
In the context of websites, web servers can refer to the hardware or software, or both of them working together. 

**Hardware:**
On the hardware side, a web server is a computer that stores web server software and a website's component files like pictures, html, css, and javascript files. This web server is also able to exchange data between other devices connected to the web. 

When referring to a computer as a web server you may think of a computer like your laptop or PC at home and yes these are computers that can serve as web servers like shown in image 1. Web servers can be run on any computing device that is able to run the web server software. Web servers are also commonly run on computers specifically designed to serve the purpose as a server which are called rack servers that are encased in a large cabinet like shown in image 2.

![Image of  desktop computer](source/Backend/assets/desktop-image.jpg.) 	![Image of server rack](source/Backend/assets/server-rack-image.png)

**Software:**
On the software side, a web server includes several parts that control how web users access the hosted files on the server. At a minimum this is an HTTP server. An HTTP server is software that understands URLs (web addresses) and HTTP(Hypertext Transfer Protocol). The HTTP server can be accessed through the domain names of the websites it stores, and it delivers the content of these hosted websites to the user’s end. 

The internet is made up of protocols which are sets of rules that govern the communication and exchange of data over the internet. The HTTP protocol is what your browser uses to view webpages. 

**HTTP Explanation:**
At the most basic level, whenever a web browser needs a file that is hosted on a web server, the browser requests the file via HTTP. When the request reaches the correct (hardware) web server, the (software) HTTP server accepts the request, finds the requested document, and sends it back to the browser, also through HTTP. (If the server doesn't find the requested document, it returns a 404 response instead.)

![Image of HTTP request](source/Backend/assets/HTTP-request-image.png)

**To publish a website, you need either a static or a dynamic web server:**

A static web server consists of a computer (hardware) with an HTTP server (software). We call it "static" because the server sends its hosted files as-is to your browser.
 
A dynamic web server consists of a static web server plus extra software, most commonly an application server and a database. We call it "dynamic" because the application server updates the hosted files before sending content to your browser via the HTTP server.

For example, to produce the final webpages you see in the browser, the application server might fill an HTML template with content from a database. Sites like Wikipedia have thousands of web pages. Typically, these kinds of sites are composed of only a few HTML templates and a giant database, rather than thousands of static HTML documents. This setup makes it easier to maintain and deliver the content.

**To sum up Web Servers and analogy:**

For example let's say you the user is using a computer and have the google browser open. You want to visit the website https://ucsd.edu/  and when you click the link, your computer sends an HTTP request to the UCSD webserver. The HTTP server part of the web server looks for the files that make up the UCSD website then the web server sends the files back to your browser where they can be viewed.  

An analogy to think about this is like a restaurant. In the restaurant the kitchen would be considered the web server. Just like how the kitchen receives orders from the waitstaff (the users computer), prepares the food (processes the request) and then sends them back out to the waitstaff to be delivered to the customers (users web browser).

![Image web server kitchen analogy](source/Backend/assets/web-server-kitchen-image.png)




[Previous: Backend](../Backend){: .float-left .v-align-text-top}
[Next: Databases](Databases){: .float-right .v-align-text-top}
