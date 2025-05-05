---
layout: page
title: Web Frameworks
permalink: web_frameworks
show-title: true
---

## The Two Web Frameworks

There are many web frameworks that can build a database and a website that can query the database and display data to users. In this project, I am using and comparing two of them: Django, which is written in Python, and Nodejs/Angular, which is written in JavaScript. 

- **Django (Python)**

The Django framework is a relatively simple (flat) web framework that does not have an API or a front end. As this data flow chart shows, the data stored in the back end will be directly sent to the webpage filtered by the user’s queries. In other words, whenever a user browses or searches for data on the website, the database back end is directly queried, and the data that fulfill the user’s criteria are directly fed to the HTML templates and displayed. 

<p align="center">
    <img src="assets/img/django.png" width="700"/>
</p>

This kind of flat framework has both advantages and potential problems. One obvious advantage is that because of its **simplicity**, a Django website is easier to learn and to build. The process of constructing a database website with Django is very straightforward: firstly, construct the database (create tables and associate tables); secondly, design different functions to query and filter the data; thirdly, write HTML templates and CSS files to display the data. For data testing or development purposes, it would be convenient to set up a Django website where developers can look at the relationship between different types of data. Additionally, Django is also a handy framework for a public-facing database website for temporary use (I will explain why in the next paragraph).

However, since the Django framework lacks an API, nor does it have a front end, its **reusability** and **flexibility** are very limited. In terms of reusability, since Django does not have an API that separates the database and the webpage, it could be problematic if the structure of the database changes. For example, if due to some unforeseen reasons, data entries become more complex and new tables need to be added a year after the original site was built, then a huge part of the code related to the webpage needs to be modified as well. Similarly, if a developer wants to improve how data are displayed on the webpage, it is very likely as well that they will need to redesign and restructure the database. In other words, the code of the Django framework is not so reusable in the face of potential changes; a small structural change may necessitate redoing the entire project. As a result, from the perspective of project maintenance, Django is not an ideal choice for long-term projects that have ongoing needs for website/data improvement and are going to be maintained by multiple people.

In terms of flexibility, as Django does not have a front end, the interface designed by Django can be less dynamic and less interactive than the ones designed by Angular. What’s more, the webpages in Django are not systematically modularized, making it more difficult to design webpages with complex components and functions. Therefore, if the dataset is large, involves a good number of types of data, and the relationship between data is complex, then it might be challenging to use Django to search for and display the data.

In sum, Django is a handy choice if the database is only for short-term use, the dataset is relatively small, and the relationship between various types of data is not too complex.


- **Nodejs/Angular (JavaScript)**

Nodejs is a runtime JavaScript environment primarily used for backend development, and Angular is an open-source web framework developed by Google. As the following chart illustrates, this more complex database website consists of three parts: the backend (Nodejs), the API (Nodejs), and the frontend (Angular).

<p align="center">
    <img src="assets/img/workflow.png" width="700"/>
</p>

As mentioned before, the backend is written in JavaScript with Nodejs. It performs almost the same function as the database in the Django framework: it stores all the metadata and the relations between different types of metadata. 

The API, which stands for Application Programming Interface, is developed together with the backend. It handles the server-side logic and data management, or in other words, it defines different functions and routes for fetching data or performing actions. 

The frontend is a web interface that displays data and a place where users browse, filter, and query data. The frontend itself does not have any data stored inside; instead, when a user puts in some searching criteria through the web interface (for example, a church name and a diocese), it sends a query request to the API, which then queries the backend and sends back the data it retrieves to the frontend to be displayed. In this project, I am using Angular for the frontend.

Compared with the Django framework, this hierarchical web framework of backend-API-frontend is much more powerful and flexible. Since this webpage is written with Angular and is a single-page app, it is dynamic and is able to respond to users’ requests on-the-fly, without having to jump to and load a new page. For example, the moment a user starts typing in a filter bar, the webpage instantaneously changes and presents the corresponding data that matches the filtering criteria.
In addition, as mentioned before, separating the backend and the frontend makes it easier to manage and maintain the project in the longer term. Changes in the backend – for instance, data association logic or ways of fetching data – will not affect the frontend as long as the data it feeds back to the frontend remains in the same format. 

On the other hand, however, the problem with this more complex structure is also obvious – the learning cycle is longer and it takes longer to build the website. Thus, it may not be very efficient when the dataset is small and does not require a very advanced website. 
