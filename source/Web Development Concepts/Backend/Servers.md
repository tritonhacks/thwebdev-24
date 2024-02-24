---
layout: default
title: Servers
nav_order: 2
permalink: Web Development Concepts/Backend/Servers
grand_parent: Web Development Concepts
parent: Backend
has_children: false
---

# What are Servers?
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

Before we can dive into what a server technically is, we need to understand how computers communicate with each other. Humans communicate with languages, but computers communicate with each other using what we call the Hypertext Transfer Protocol (HTTP) 📡.

## Understanding Hypertext Transfer Protocol (HTTP) 🖥️
HTTP is the foundational protocol used by the internet. It defines the rules and standards for transmitting and receiving data over the internet 🌍. Imagine it as the common language that computers use to talk to one another. When you want to visit a webpage, your computer sends an HTTP request to the server where that page lives, asking for the page to be sent to you 📤. The server, understanding your request through HTTP, responds by sending the webpage back to your computer in the form of different files which your browser renders for you 📥.

When you enter a restaurant 🍽️, imagine it's like typing a website address into your browser. In this scenario, you (the customer) are like the browser, or the client, stepping into the restaurant to have a meal. This process is similar to using HTTP on the internet, which is the method your browser uses to communicate your request in a language that the website's server (think of it as the kitchen where your meal is prepared 🍳) can understand.

Once the website's server receives your letter 📨, it sends back a package containing everything you need to visit the website, such as text, images, and videos. This package is also sent via HTTP, ensuring that your browser can understand and display the website correctly for you 🖥️.

![HTTP Image](../../source/assets/images/http.png)

## Servers: The Backbone of a Website 🍽️
Let's dive a bit deeper into what a server is on the internet, drawing from our restaurant analogy. In a restaurant, your server plays a crucial role: guiding you to your seat, taking your meal order, and delivering your food to you. But remember, they don't cook the food; that's the chef's job 🧑‍🍳.

However, in the digital "restaurants" that are the internet, servers operate a bit differently. Imagine you're craving to view a specific webpage, much like how you'd order a dish at a restaurant 📜. When you type a website's address into your browser, it's similar to placing your order. This is where the web server steps in, acting not just as your server but also as the chef 🚀.

A web server is essentially a computer program that's ready to fulfill your order. But instead of heading to the kitchen, it searches its digital shelves for the webpage you've requested. Once found, it prepares this "digital dish" by gathering all the necessary files — text, images, videos — and sends them directly to your screen 📲.

What sets a web server apart from a restaurant server is its ability to do it all: taking your request, preparing your order, and delivering it to you, all by itself. In this digital dining experience, the server is the multitasking maestro, ensuring you get exactly what you asked for, straight to your device. This makes the web server an all-in-one package — both the server and chef of the internet world, ready to cater to your digital cravings 🌐.

![Image web server kitchen analogy](../../source/assets/images/web-server-kitchen-image.jpg)

[Previous: Backend](../Backend){: .float-left .v-align-text-top}
[Next: Databases](Databases){: .float-right .v-align-text-top}
