---
layout: default
title: RESTful Routes
nav_order: 4
permalink: Web Development Concepts/Backend/RESTful
grand_parent: Web Development Concepts
parent: Backend
has_children: false
---

# What does RESTful mean?
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---
Let's continue with the analogy of a restaurant. Representation State Transfer are the set of rules for how to order, prepare, and serve those dishes efficiently. 

## Understanding Representation State Transfer
Imagine you go to a restaurant and order a burger 🍔. Each time you order, you have to tell the waiter exactly what you want. You can't just say "the usual" and expect them to remember your last order. This is like how in RESTful services, every request you make needs to have all the information necessary 📝 to complete that request without relying on previous interactions.

This is like having a menu with specific items listed 📖. Just as you use the menu to select your meal in a standard way, RESTful services use standard methods (like GET for viewing 👀, POST for creating ✏️, PUT for updating 🔁, and DELETE for removing ❌) to interact with resources (the data or services they want to use).

Think of the kitchen and waiter as the server and yourself as the client. You (the client) order your food through the waiter 📋. The kitchen prepares your food 🍳. You don't need to know how the kitchen operates to get your meal, and the kitchen doesn't need to know who you are to prepare your meal. This separation allows you to enjoy your meal without worrying about how it's made 🥘, and the kitchen can focus on making food without serving tables.

## API
text

talk about API

![API Analogy](../../source/assets/images/api.avif)


[Previous: Databases](Databases){: .float-left .v-align-text-top}
[Next: Tutorials](../../Tutorials){: .float-right .v-align-text-top}
