---
layout: page
title: Tableau Public
---

## Introduction

The goal of today is continue to develop your comfort with working with, analyzing, and visualizing data using Tableau Public. For the purposes of today, you're going to be using a dataset published by some lame professor at CU Denver: [US Post Offices](https://cblevins.github.io/us-post-offices/).

## Get to know the data 

- Take 5-7 minutes to scan through [the data website](https://cblevins.github.io/us-post-offices/) and in particular look at the section of the data biography ["What's in the data?"](https://cblevins.github.io/us-post-offices/data-biography/#whats-in-the-data:~:text=What%E2%80%99s%20in%20the%20data%3F).
- Download the files: `us-post-offices-random-coords` (your main data file) and `us-post-offices-data-dictionary` (metadata about that file) from [Harvard Dataverse](https://doi.org/10.7910/DVN/NUKCNA), saving them into your class folder on your computer. Hint: you want both of these to be downloaded as CSV files, which you can do by clicking the Access File icon and then clicking Original File Format (Comma Separated Values).
- Open `us-post-offices-data-dictionary.csv` on your computer and familiarize yourself with the different columns in the main dataset `us-post-offices-random-coords`. 

## Explore the data in Tableau Public

- Connect to the data source on your computer, which should be downloaded as `us-post-offices-random-coords.csv`.
- Spend a few minutes dragging and dropping different column names onto a worksheet so you can start to get a feel for the data.
- As an entire class we will walk through the steps to answer this question:
	- In what year did the state of Colorado experience the largest number of post office closures (hint: use the `Discontinued` field)? How many post offices closed that year?

## Visualize the data

Sheet 1:

- Choose a state OTHER than Colorado
- Make a bar chart showing how many new post offices were established each year only for the state you selected (hint: use the `Filters` tool)
- Annotate the "peak" of the graph - ie. the year when the most post offices opened in the state.
- Change the labels for the Y axis and X axis to better explain them to a reader

Sheet 2:

- Make a map of all the post offices in the dataset
- Only show post offices on the map from one state of your choosing using the `Filters` tool.
- Use the `Pages` feature to allow a user to "flip" through and see new post offices that were `Established` each year (play around with the `Show history` feature)
- Add information about the post office's name, year it opened, and year it closed in the `Tooltip` so that a user can click on a point and get this information.
- Color all the post offices that have semi-random coordinates light blue. Hint: use the `RandomCoordinatesFlag` field.


## Publish the data online

- Embed your map into a new post on your Wordpress sandbox site. You can use [these instructions](https://youtu.be/LVmpQ2c0fmg?t=269) or try to do the following:
  - Make a new post or page in Wordpress
  - Insert a new block and make sure its type is set to `Custom HTML`
  - Publish your Tableau Public workbook online
  - Open your Tableau Public workbook through your browser and click on the Share icon in the bottom right (3 circles with lines connecting them).
  - Click the embed code text book and copy it
  - Paste it into your Wordpress Custom HTML block. It should look like a bunch of jumbled text that starts with `<div class=`. This is the Javascript code that is going to allow you to display your Tableau visualization inside a webpage.
- If it's not working for you ask your classmates or Professor Blevins for help. 

## Bonus Tableau Practice

Try to create a chart/map that answers the following questions:

- What are some of the most common names for post offices in the dataset?
- Which states had the most post offices operating within them during the 1900s? Make a map with each state shaded according to how many post offices operated in that state during the 1900s.
- In what year did the first post office open in Alaska? What was its name?