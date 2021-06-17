---
layout: post
title:      "World Hopper - A React/Redux Project"
date:       2021-06-17 01:13:55 +0000
permalink:  world_hopper_-_a_react_redux_project
---


We made it! Well kind of made it, one more review to go!

For my final project at Flatiron school, I created an app using Rails as the backend and React/Redux for the frontend. This was hands down the most challenging project of all, yet probably the most fun. The projects are finally starting to look like the UIs we are used to seeing.

My project is catered to little observers, kids who are curious to know more about the world they live in. Through my app kids can browse through all the countries in our little world, they get to know select countries to learn more details about them.

Throughout this project I came across a couple of bumps so I decided to write about them briefly so that maybe this blog would save someone some precious debugging time;

* The first issue was with how the data I received from my fetch request was being handled. The app was trying to render the elements before the promise was being fulfilled. The isLoading() came to the rescue, it returns a Boolean and the app would only get to proceed to rendering when this Boolean is set to False.

* The second issue I faced was with passing props from one component to the other, setting up a Parent/Child relation between the components didn’t provide the results I was looking for. I then resorted to having a Function component and utilizing Hooks to access these props through the component. To be more specific, I got to use useSelector and useDispatch to grab the props from the global state and to perform the dispatch actions.

* The last issue worth mentioning was with the Flash Card Game I build for the app; duplicates of the data were being pushed and I would end up with hundreds of arrays of data. to fix this issue I resorted to creating an empty array and using a conditional that my fetch action would only be fired when this array is empty. That way I avoided the problem of data duplication.

If anyone comes across this one day, I hope I have been of some help! Good luck to you and us!
