+++
title = 'Point Trackers'
date = 2024-06-21T14:38:33+02:00
draft = false
type = 'blog'
+++

# Point Trackers
I have built three different point tracker programs for schools. These points trackers were integral parts of either 
the house team system or the SW-PBIS program at the school. Each of these three programs has been customized to 
the school's needs, but they all were built on a few key concepts.

# SSI Scholar Dollars
This was my earliest version of a point tracker. This iteration was in support of an SW-PBIS program, specifically
awarding students for their good behavior outside of classroom. When I arrived at the school, they had implemented a 
school-wide token economy through checks written by the teacher to the student, who then had to carry the check to the 
office to deposit it into their account. This method was cumbersome and led to teachers not utilizing the system and 
students not cashing in their checks. Several of my students were actually using the checks as bookmarks because they 
were too difficult to turn in for actual rewards.

Over the summer, I wrote a website which used QR codes to allow teachers to award students directly through their 
phones. Students carried a QR code with them and teachers could scan that QR code, so they could award or spend their 
scholar dollars. This program led to a nearly 3000% increase in the use of the token economy system (as measured by 
awards given and rewards claimed) over the course of a single semester and continues to be used to this day. It also 
helped reduce a regular issue with attendance in the school.

Homeroom attendance was spotty and inconsistent prior to this system because homeroom attendance did not impact 
graduation, so students didn’t see the benefit of attending, only the consequences of skipping (which they felt were 
worth the cost). But by awarding scholar dollars for homeroom attendance, we were able to reduce skipped homerooms to 
nearly zero over the course of one year. Homeroom attendance at the school continues to be high, in large part because 
of the role this program plays in their token economy system.

# RIS MS House Team Points
RIS was using a Google Sheet to track their points, but it was difficult for students to see the live scores as house
events were running. Additionally, there were concerns about allowing access to the spreadsheet to the student council
in case they accidentally deleted something.

As the most important concerns were updating the view, this design focused on the graphical chart. The data entry was
handled entirely within a pre-built solution, allowing me to concentrate development time on the most important part of
the project. The site was first rolled out at our Knowledge Bowl just before Christmas break. With a team of students
logged into the site to do data entry, we had a live chart of the rankings after each question as the knowledge bowl
progressed. It really drove up the engagement and excitment in what is already an exciting day for the MS.

# SJA ES House Team Points
The Point Tracker that I built for SJA combined ideas from both of the previous two. While points would be awarded by
individual teachers rather than house events, they still wanted a live tracker to use during their weekly assembly.
To simplify management of the accounts, a single sign-on system was incorporated which prevents students from creating
accounts while still allowing teachers to sign in easily. This also simplifies onboarding new ES teachers because
accounts do not need to be created manually for them. This system has been an integral part of their House Team 
implementation and is used regularly.

# Developer's Notes
Each of these tools has been built using Python3 and hosted on either PythonAnywhere or Heroku. For future development,
I would likely migrate to a different language and tech stack, specifically a Clojure based deployment. This is because
Clojure allows you to use the same language for the server and for the client, as ClojureScript is a version of the
language that can be converted to JavaScript to run in the webpage. 

