---
layout: default
title: Databases
nav_order: 3
permalink: Web Development Concepts/Backend/Databases
grand_parent: Web Development Concepts
parent: Backend
has_children: false
---

# What are Databases?
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

Databases are essential for managing and organizing data in a way that makes it easy to access, manage, and update 🔄. Think about the restaurant analogy 🍽. Before you can enjoy a meal, the kitchen needs all sorts of things like ingredients 🥦, spices 🌶, and cooking tools 🍳. A database holds all the bits and pieces of data 📊 that a computer program needs to work, all organized so it's easy to find and use, just like how a kitchen organizes everything to cook your food. In our web development case 🌐, a database may store data such as user-specific information 👤.

## Relational and Non-Relational Databases 🗂
There are several kinds of database, but the only two you need to understand for a introductory to databases are relational and non-relational databases. 

### Relational Database 📊
Relational databases store data in tables, sort of like grids 📈. Each table is for a different category of information. For example, one table for customer info 🧑‍💼 and another for orders 📝. These tables can link to each other through shared information, like if a customer places an order, there's a way to see that in both the customer and order tables.

They're great when your data is structured and consistent 🏛. This means you know exactly what information you need to store ahead of time, like names, addresses, or product orders. They're used a lot in systems that need to keep track of things precisely, such as bank transactions 💰 or school records 🏫.

Imagine a well-organized binder with different sections for each subject in school 📚. Each section has pages that follow the same format, making it easy to find and understand information. If you need to see how your math grades relate to your overall GPA, you can easily flip through the binder to find and connect that information 🔍.

### Non-Relational Databases 🌀
Non-relational databases, or NoSQL databases, are more flexible in how they store data. They can handle a mix of structured and unstructured data, like text 📝, social media posts 💬, or even videos 🎥. They don't require a fixed table structure and can easily scale to handle huge amounts of data 📈.

These are great for big data applications or services that collect a lot of user-generated content, like social media platforms 📱 or e-commerce sites with customer reviews 🛒. They can quickly adapt to changes in the type of data being stored and can handle massive amounts of data 🌐.

Think of a big, expandable folder 📂 that you can throw all sorts of notes into, whether they're written neatly on lined paper 📄 or quickly jotted on napkins 🍽. You don't have to organize every piece of information in the same way, and you can keep adding more notes without worrying about running out of space or messing up the order 🔄.

![Kitchen Database Analogy](../../source/assets/images/database_kitchen.jpg)

[Previous: Servers](Servers){: .float-left .v-align-text-top}
[Next: RESTful](RESTful){: .float-right .v-align-text-top}
