---
layout: page
permalink: /story/
---

# The Development of Santos Traffic Platform

In 2014, Olin College of Engineering and the Santos Family Foundation begin their collaboration on a multi-year project working to improve traffic safety. The first part of the project began in June of 2014, and laid the ground work to which future teams would build. This project was transferred to the Senior Capstone program (SCOPE) at Olin, where a team of four to six senior engineering students would dedicate a full year to the project.

## Senior Capstone Project 2014-2015

The 2014-2015 SCOPE team began work by conducting user interviews and determining the best direction to take the project. A majority of the year was spent on defining the project so future teams could begin technical work. This team discovered intersections to be a major pain point and began ideation on how to work in this space.

## Senior Capstone Project 2015-2016

Using the previous year's findings, the 2015-2016 SCOPE team conducted in-depth interviews with advocacy groups and traffic engineers, who they identified to be the major change-makers in intersection infrastructure. After gathering a surplus of information, they began developing a software system which could produce safety metrics of any intersection. To accomplish this, the team adopted a pre-existing traffic analysis library produced by Dr. Nicolas Saunier from Polytechnic Institute of Montreal. His library provided video analysis functions which use OpenCV to create vehicle counts, speeds, and trajectories. From these speeds and trajectories, another layer of analysis can be run to determine collision data and near miss counts. The team managed to produce a rough User Interface which called these functions and aided the user in understanding the data from the collected video.

## Senior Capstone Project 2016-2017

Our team picked up the project from the stopping point of the 2015-2016 team. We immediately began work on the User Interface, using it to better understand functionality of the underlying library.

### Our First Traffic Study

We began a traffic study in Needham, MA, receiving permission from a local shop owner, Harvey's Hardware.  A camera was placed on top of the roof to view the intersection. to put a camera on top of their roof with view of the intersection. Ten hours of usable data from the intersection was collected before battery power was lost. After the analysis was completed, we presented our data to the Needham Heights Neighborhood Association to show them our findings and began the conversation of how to most effectively use the data we gathered for the community.

### Separation of User and Process

One of our immediate challenges to utilizing the software from the 2015-2016 SCOPE team was the difficulty of installing both the user interface and the traffic analysis library which was provided by Dr. Saunier. Many potential users would be unable to finish the installation, due to the errors that would prevent the software from running. Our solution was to move the processing and analysis libary to a cloud-based platform. Users would no longer be required to download and install this portion of the software. We developed a Vagrant image with all the software and dependencies required to make the user interface functional. Using the Tornado framework, we developed an API for the user interface to connect to the cloud processing functions. This has several benefits: developers can use the API to make calls to the server, the server components can be spun up in AWS on multiple machines, and developers can create their own front-end for different use cases we have not thought of..

### Code for Boston

As our project came to a close, we looked for interested people who wanted to continue the technical development of our software. Code for Boston is a group of civic-minded developers who hack on open source projects in their free time. We have approached them about adding the Santos Traffic Platform to their list of projects and the group is interested. If they decide to adopt this project, development and refinement can continue.

### Creating CrossRoad Optics, a Civic-Focused Company

Two members of the 2016-2017 SCOPE team have been accepted into the Summer Venture Program with Babson College. CrossRoad Optics, a business venture utilizing the software created during SCOPE was created. In this capacity, the SCOPE project will continue under the direction of CrossRoad Optics.
