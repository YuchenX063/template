---
layout: page
title: Database
permalink: database
show-title: true
---

Since both websites are not running on a server right now, I am illustrating them with screenshots of how they look like when running locally. This site will be updated once I put the website onto a server.

## The Django website

<p align="center">
    <img src="assets/img/django website.png" width="700"/>
  <em>Home Page</em>
</p>

If we click St. Mary's in 1870 Albany, we land on this page: 
<p align="center">
    <img src="assets/img/django-inst-detail.png" width="700"/>
  <em>The detail page of St. Mary's</em>
</p>

Then, by clicking the name "Rev. C. Walworth," we can browse this person's detail page, which contains information about this person in the year 1870:
<p align="center">
    <img src="assets/img/django-pers-detail.png" width="700"/>
  <em>The detail page of Rev. C. Walworth</em>
</p>

We can also use the search bars to search for or filter institutions:
<p align="center">
    <img src="assets/img/django-search.png" width="700"/>
  <em>The search result page of St. Mary's in Boston and related people</em>
</p>

Or search by person name:
<p align="center">
    <img src="assets/img/django-search-pers.png" width="700"/>
  <em>The search result page of people named John and related institutions</em>
</p>


## The Nodejs/Angular website

Below is the browse institution page of the Nodejs website. There are two major differences between the new website and the old one. First, instead of displaying institutions and people parallelly in two columns, I chose to have two separate pages: one for institutions, and one for people. Second, on this more advanced website, I no longer treat an institution in a specific year as an individual entity. Instead, I treat IDs as unique entities – in other words, the institutions on this page are grouped by their ID, and by clicking their name, users can view the more detailed page that has all other information about the institution throughout different years. I will elaborate on the decision-making process in the reflection section.
<p align="center">
    <img src="assets/img/node_website.png" width="700"/>
  <em>Browse Institution Page</em>
</p>

The institution detail page contains all the metadata of a specific institution. The default page (“All years”) displays the metadata of the latest year of that institution (in this case, year 1870) and all the relevant people and institutions across various years. 
<p align="center">
    <img src="assets/img/inst-detail.png" width="700"/>
  <em>The detail page (all years) of Cathedral Chapel of the Holy Cross</em>
</p>

If a user hits a year button – for example, 1869 – then they can view the metadata of that specific year: language, diocese, city, relevant people in 1869, etc.
<p align="center">
    <img src="assets/img/inst-detail-year.png" width="700"/>
  <em>The detail page (1869) of Cathedral Chapel of the Holy Cross</em>
</p>

On the previous page, if we click the person “Rev. P.J.Power,” we can access their person detail page as well:
<p align="center">
    <img src="assets/img/pers-detail.png" width="700"/>
  <em>The detail page Rev. P.J.Power</em>
</p>

There is also a browse people page similar to the browse institution page.
<p align="center">
    <img src="assets/img/browse-people.png" width="700"/>
  <em>The browse people page</em>
</p>

On both the browse institution page and the browse people page, users can explore and search for the institution/people they are interested in by putting in filtering criteria in the search bars.
<p align="center">
    <img src="assets/img/search-inst.png" width="700"/>
  <em>The search result of St. John's in Boston</em>
</p>

For a reflections page, [see here](https://yuchenx063.github.io/template/reflections).
