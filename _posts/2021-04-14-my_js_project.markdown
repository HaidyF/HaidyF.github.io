---
layout: post
title:      "My JS Project "
date:       2021-04-14 05:38:27 +0000
permalink:  my_js_project
---

We have reached the project for module 4, feels unreal how fast time flew by. 

For this project I have decided to build a single page application that can be used as a portfolio website for architects. The first and most important step of every project is the planning, spend as much time as you need planning your project. 

When planning, I first think of what my user story would be, who would use my app and why, what features do I want my app to have and a design that would make my app appealing to the user. At this point I only focus on the use rather than the implementation, there will be plenty of time to think, test and execute the implementation later on.

After, I start thinking of my models and their associations, in this app I had a project Category model that has_many of the Project model. I mapped everything out using draw.io and came up with the schema. I always forward my schema to our cohort lead to make sure the app is meeting the basic requirments before proceeding.

It's finally time to set up your project and code, I created my repositories for both my backend and frontend and I was ready to start using my Rails generators to create my project and it's models and right away listed my associations. Afterwards I tackled generating the database, seeding some data for it and migrating. later on I finished my resources and controllers. Make sure to disable CORS and add it's gem.

I then proceeded to work on my frontend, and this when I felt completely lost and had no idea where to start - It's funny how Rails now feels like a home-. And of course at time of doubt we resort to google, I watched multiple project build videos and read lots of blog posts to get a sense on how and in what order should the frontend be executed. 

I went ahead and created my classes with their constructors, then created my first fetch and event listener. Then created my form to creating projects with anoher event listener for the submit button. Later, I decided to have my rendering function as a class function in my project.js rather than in the index.js to make my app more organized and efficient. 

Now with my GET fetch request completed, I went ahead and created my second fetch request; a POST method request to enable creating new instance of my Project class. One very important thing I forgot was to add "event.preventDefault()" which basically cancels the default action of an event. Through all of this debugger was my best friend, I had breaks in almost every line of code, taking them one at a time, trying to fix all the problems that came up.

Another bump in the road I had here which needed some google was that my create function was working but the new project would only show when the page is refreshed. After some googling I was able to find the location.reload() method which took care of this problem. 

Only two CRUD actions were required for this project, but I felt like the app would not be complete without the option to DELETE instance. I decided to add the delete functionality and there went my third fetch request; a DELETE method request which surprisingly took the longest time to get to work, I added the event listener and handled removing the project from the DOM and it was still not working. What was missing was my function which iterates over the projects and removes the one targeted.

With all three fetch requests functioning, I have been feeling a little more comfortable and trying to figure out the CSS for my app and trying to make it look more appealing. Even though I know that the app's design will need some improvement, I am enjoying this process and will probably be coming back and making all my apps look more sophisticated.



