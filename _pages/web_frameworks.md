---
layout: page
title: Web Frameworks
permalink: web_frameworks
show-title: true
---

## The Two Web Frameworks

There are many web frameworks that can build a database as well as a website that can query the database and display data to users. In this project, I am using and comparing two of them: Django, which is written in Python, and Nodejs/Angular, which are written in JavaScript. 

- Django (Python)

The Django framework is a relatively simple (flat) web framework that does not have an API or a front end. As this data flow chart shows, the data stored in the back end will be directly sent to the webpage filtered by the user’s queries. In other words, whenever a user browses or searches for data in the website, the database back end is directly queried, and the data that fulfill the user’s criteria are directly fed to the HTML templates and displayed. 

<p align="center">
    <img src="assets/img/django.png" width="700"/>
</p>

This kind of flat framework has both advantages and potential problems. One obvious advantage is that because of its simplicity, a Django website is easier to learn and to build. The process of constructing a database website with Django is very straightforward: firstly, construct the database; secondly, design the views and different ways of querying the data; thirdly, write the HTML and CSS files to display the data. Therefore, for data testing or development use, it would be convenient to set up a Django website where developers can look at the relationship between different types of data; Django could also be used for a public-facing database website for temporary use. 

- Nodejs/Angular (JavaScript)

