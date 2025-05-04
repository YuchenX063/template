---
layout: page
title: Reflections
permalink: reflections
show-title: true
---

Before starting to build the frontend, I assumed that the biggest decision a tech person needs to make in a DH project is which technical approach to take to build the actual website/map/model etc. However, in the process of creating the webpage and seriously thinking about how I want to display the data, I realized that there are much more equally important decisions to make, and some of them can be tough. Therefore, in the reflection section of this website, I would like to focus on what decisions I made and I will try to explain why I made those decisions.

## Technical approaches

As mentioned in the section Methodologies – Web Frameworks, the two web frameworks Django and Node/Angular both have advantages and disadvantages. Therefore, when making the decision of which framework to use, it is necessary to consider the project’s life cycle, project maintenance expectations, as well as current project needs. As for the Almanacs project, Node/Angular is apparently a more sustainable choice. First, as students continue to collect data from more years, unexpected data type or data format may appear (either in almanacs that are too early or too late). As a result, the backend and the frontend may frequently need to be improved. If the backend and the frontend are separated, it is more convenient to make changes in either end without affecting the performativity of another end than having them all messed together. Second, we can also publish the API and allow other web developers to use it to interact with the database in the ways they want. This can even be an instructive opportunity in a digital humanities class when teaching/introducing frontend development. Last but not least, since Angular is more specialized in frontend development, its webpage has more flexibility and interactivity than a Django webpage. Consequently, the Node/Angular framework is more ideal than a flat website.

## How to display the data
How to display the data – or more specifically, how to name the data as it is displayed – is a big issue I have encountered when building the frontend. For institutions, for example, there are two possible options to display their name. One, to give each institution a generic name, use that name to represent the institution, and display each institution individually; or alternatively, to display the combination of institution and year, and display the institution’s name as it is in the almanac record. In the previous Django site, I chose to use the latter way of naming and representing the data. However, users cannot have a more comprehensive view of the metadata of a specific institution across several years. They can only browse one institution in one year at a time. This makes it very hard to really track the change of the metadata of the institutions throughout different years. 

## About team work

