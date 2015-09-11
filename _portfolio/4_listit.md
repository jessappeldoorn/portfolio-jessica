---
layout: post
title: List.it
thumbnail-path: "img/listItMockup.jpg"
short-description: Create tasks with an expiration date. 

---

{:.center}
![]({{ site.baseurl }}/img/listItMockup.jpg)

---
[WEBSITE](http://just-list-it.herokuapp.com/ "Website")
---
[SOURCE CODE](https://github.com/jessappeldoorn/List.it "Code")

## Case Study Explanation

To-do lists are notorious for collecting junk - tasks that you want to remember, but constantly reprioritize. To solve the problem of to-do list clutter, list.it will manage your to-do lists by automatically deleting tasks that have not been completed after seven days; after-all, if your task is not important enough to be completed in seven days, it doesn't belong on your to-do list.  

I built this application as part of my coursework through the Bloc Web Development Program. The app was built using AngularJS, HTML5, SASS(CSS3) with Bootstrap, the Firebase API and Grunt.

## Use Case + Solution

User Story      | Implementation
------------- | -------------
As a user, I want my tasks synced with a persistent backend  | Synchronize Data (an Array of Tasks) With Firebase.
As a user, I want to see my active tasks in a list as my default view | Configure ui-router and controller to handle views and display tasks in a list using ngRepeat.
As a user, I want completed tasks and tasks older than seven days hidden from my main task views automatically | Use ngHide or ngShow to keep the logic out of the controller and view.
As a user, I want expired and completed tasks presented in a separate view | Create a separate state, template, controller and register them with your ui-router-driven routes.
As a user, I want to submit new tasks with a description, priority level and three states: expired, completed or active  | Create an input with an ngModel tied to a $scope model at the top of the list. Allow the user to save the task by clicking a button or link. Use a dropdown to hold all of the priority levels and choose one before submitting the task. Use a $scope method to call the $add() method on the array to sync the task with Firebase and refresh.
As a user, I want to mark tasks as complete | Add a button or link inline with the task item. Include the trigger within the ngRepeat block so it will be scoped to the clicked item.

<!-- ## Results

The Timer is the core feature of pulse & pause. Users can immediately start using the app from the landing page. It displays a timer for working/breaking and a start/reset button. When each interval is completed, a bell will sound and the timer will automatically continue it's cycle through 4 work/break sessions, unless the user chooses to reset.   

For added features, a user can login via Facebook, Github, or Google+. Once logged in, a user is able to enter a task label when starting the timer. A dashboard link is displayed in the navigation bar, which stores the users data. Tasks will be shown in the dashboard with relevant information, such as a date completed and number of working intervals. (User authentication is currently a work in progress and will be updated in a future deployment).

The site also contains an information section describing how to best use the app, for ultimate productivity. -->

---
[WEBSITE](http://just-list-it.herokuapp.com/ "Website")
---
[SOURCE CODE](https://github.com/jessappeldoorn/List.it "Code")

