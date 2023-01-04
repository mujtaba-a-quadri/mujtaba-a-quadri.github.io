---
layout: project
type: project
image: img/wahi/WahiLogo-crop.png
title: WAHI (2021 HACC)
permalink: projects/wahi
# All dates must be YYYY-MM-DD format!
prettydt: Nov. 2021
date: 2021-11-21
labels:
  - Hackathon
  - MongoDB
  - React-Native
  - Meteor
  - Web App
  - Mobile app
summary: A marine animal reporting app and website; my team of 5's submission for the 2021 HACC Hackathon.
---

<figure class="figure float-end">
  <img width="550px" style="padding-left: 2rem" class="figure-img img-fluid img-responsive" src="../img/wahi/AppHome.jpeg">
  <figcaption style="padding-left: 2rem" class="figure-caption">The homepage of our mobile app</figcaption>
</figure>

## The Challenge 

For the [2021 HACC (Hawaii Annual Code Challenge)](https://hacc.hawaii.gov/) my group took on the challenge of implementing a marine life reporting & sighting app. HMAR (Hawaii Marine Animal Reponse) desired an app to help managing the large amount of reports they get (all through a phone line) for sightings of endangered species of birds, seals, and turtles.


## The App

Our implementation has a **mobile app** for beach-goers to submit a form for any sightings they make, with all the relevant information that HMAR volunteers need about the sighting. This data is then displayed on our webview which is exclusively for use of HMAR staff and volunteers to view reports of sightings.


For this app, I primarily worked on the Latest Reports and Confirm Related Sightings pages. The latest reports page shows all reports that users have submitted through the app, in reverse chronological order. Each row has the important info on a sighting, and a field to indicate if the report has been "Checked" and is no longer of concern. Unchecked reports can be edited or deleted by clicking on the animal type, and appear at the top of the sorting regardless of date.


The Confirm Related Sightings page has a similar view, with rows of sightings in a table displaying the important info. These sightings are in groups (with alternating colors) that were detected as being similar to each other (due to factors like location or time being very similar). HMAR wanted a way to cut down on the number of duplicate reports they get, so this page allows an HMAR volunteer to distinguish at a glance whether a group of reports are the same or not. If they decide the group of reports are not actually the same sighting, they can click no, in which case the sightings will be confirmed as distinct and seperated into two rows in the Latest Reports page. Otherwise, the sightings will be grouped together as one row on the page.

## Conclusion

I learned a lot from the experience with this hackathon. After the very short Meteor Hackathon this one was very different in pace. We definitely slowed down at the start of this hackathon to catch our breath after the sprint that was the Meteor Hackathon. Once we did get this marathon (4 weeks!) started, we had to take time to learn about mobile app development, this was my first time doing anything with a mobile app, so I was thankful for my teammates who were more versed with it. On the web view side of things, the database tables for this app had more fields than I have worked with in any project. There were many pieces of data that HMAR wanted to be stored for each report, which also led to the form being quite long and complex. This made working with the data (such as when inserting or updating) very finnicky: particulary with test data which needed all the fields to be properly set.
<figure class="figure">
  <img style="width: 49%" class="figure-img img-fluid img-responsive rounded" src="../img/wahi/LatestReports.png">
  <img style="width: 49%" class="figure-img img-fluid img-responsive rounded" src="../img/wahi/ConfirmRelated.png">
  <figcaption class="figure-caption text-center">The pages I worked on (part of the web-app)</figcaption>
</figure>

<br>
<hr>
<p class="text-center">
<a target="_blank" href="https://github.com/HACC2021/DAAJ">See the GitHub repo</a>
||
<a target="_blank" href="https://daaj.meteorapp.com/">See the deployed application</a>
</p>
