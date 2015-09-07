---
layout: post
title: pulse & pause
thumbnail-path: "img/pulsePauseMockup.jpg"
short-description: Track your time working (pulsing) & breaking (pausing). 

---

{:.center}
![]({{ site.baseurl }}/img/pulsePauseMockup.jpg)

---
[WEBSITE](http://pulse-and-pause.herokuapp.com/ "Website")
---
[SOURCE CODE](https://github.com/jessappeldoorn/pulse-and-pause "Code")

## Case Study Explanation

Pulse & Pause is a web application built to help users track their time working on projects; it's based on the Pomodoro Technique, which aims to increase your work productivity and quality. In its simplest form, you time your work in 25-minute intervals, with five-minute breaks in between; it includes 3 timers: Work, Short Break, and Long Break. During a 25-minute session, you focus on a task - during a break, you do not do anything related to work!

When implemented with discipline, pulse & pause can be a powerful tool to help increase your productivity. I built this application as part of my coursework through the Bloc Web Development Program. The app was built using AngularJS, HTML5, SASS(CSS3) with Bootstrap, the Firebase API and Grunt.

<!-- ## Use Case
* As a user, I want to start and reset a longer, 30-minute break after every four completed work sessions
* As a user, I want to record completed tasks -->

## Use Case + Solution
 
User Story      | Implementation
------------- | -------------
As a user, I want to start and reset a 25-minute work session  | Create a button with the ngClick directive to trigger a function that starts/resets the timer. Use an ngBind directive to handle the button text. Use Angular's $interval service to execute a function that updates the remaining time every second.
As a user, I want to start and reset a five-minute break after each completed work session  | Create a boolean variable to control the state of the timer. Use the ngShow or ngHide directive to determine what the user sees in the view. When the timer reaches the end of a work session, modify it so the user will see this new time, and the ngShow or ngHide directive used on the buttons will pair the correct button to the timer's state.
As a user, I want to start and reset a longer, 30-minute break after every four completed work sessions  | Create a variable that holds the number of completed work sessions. Increment the count after each completed work session. When the timer reaches the end of a work session, update the time remaining by using a conditional statement to check whether the number of completed work sessions is equal to four - which would then send you to a thirty minute break. Once all sessions are complete, reset back to 0.
As a user, I want to see a live timer during work sessions and breaks | Assign the time remaining to a variable and use {{ }} markup or the ngBind directive to render the time remaining in the view. Create a filter to handle the conversion of the time remaining.
As a user, I want to hear a sound at the end of work sessions and breaks  | Add sound with Buzz and trigger a playback. Use a $watch method to register a listener callback to execute whenever the watchExpression changes. Watch the time remaining and call the .play() method on the variable that holds the sound file when the time remaining equals zero.
As a user, I want to record completed tasks | Sync with Firebase and add tasks.
   
## Results

The Timer is the core feature of pulse & pause. Users can immediately start using the app from the landing page. It displays a timer for working/breaking and a start/reset button. When each interval is completed, a bell will sound and the timer will automatically continue it's cycle through 4 work/break sessions, unless the user chooses to reset.   

For added features, a user can login via Facebook, Github, or Google+. Once logged in, a user is able to enter a task label when starting the timer. A dashboard link is displayed in the navigation bar, which stores the users data. Tasks will be shown in the dashboard with relevant information, such as a date completed and number of working intervals. 

The site also contains an information section describing how to best use the app, for ultimate productivity.

---
[WEBSITE](http://pulse-and-pause.herokuapp.com/ "Website")
---
[SOURCE CODE](https://github.com/jessappeldoorn/pulse-and-pause "Code")



  

