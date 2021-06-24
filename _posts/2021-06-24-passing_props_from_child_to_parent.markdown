---
layout: post
title:      "Passing Props From Child To Parent"
date:       2021-06-24 05:53:34 -0400
permalink:  passing_props_from_child_to_parent
---


Props allow us to pass data between components, props make our components more dynamic.

Props can easily be passed down from a Parent Component to a Child Component, but not the other way around. That’s why the communication from the Child component to the Parent component is a little more complicated. So what if we want to pass data from the Child component to the Parent component?

**Callback functions! **

Functions can be passed around from a Child component to a Parent component, the Child component can use these functions to update the Parent component’s state. In other words, we pass the data from the Child component to the Parent component as an argument into a callback function from the Parent component. The Child component in turn changes the state in the Parent component. When the state is changed, the Parent component passes the information down again as props to the Child component.

![](https://www.thecodebuzz.com/wp-content/uploads/2020/06/React-How-to-Pass-Data-From-child-Component-to-Parent-Component-394x520.jpg)

So to pass data from the Child component to the Parent component we follow these steps: 

1. We start off in the Parent component, we create a call back function that will retrieve the data that will be sent back by the Child component. This callback function will be passed to the Child component as a prop.

2. Then in the Child component, we call the Parent component's callback function using the props and we pass a value that the Parent component could react to.

3. Then, back in the Parent component we create a function that's job is to handle the value that the Parent component receives from the Child Component and storesthat new value in the Parent components state.

4. After that, we get to import the Child component and pass the the new function to the Child component as a prop.

5. Lastly, we can use the props to execute the callback function in the Parent Component.


That's basically how we can pass data from a Child component to a Parent compont if we are not using any state management libraries like Redux. Take a look at the example code below;
![](https://www.codegrepper.com/codeimages/pass-data-from-child-component-to-parent-component-react.png)



