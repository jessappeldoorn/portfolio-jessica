---
layout: post
title: kent 
thumbnail-path: "img/kentMockup.jpg"
short-description: A website for a solo artist/musician.

---

{:.center}
![]({{ site.baseurl }}/img/kentMockup.jpg)

---
[WEBSITE](http://kentappeldoorn.com/ "Website")
---
[SOURCE CODE](https://github.com/jessappeldoorn/kent-band-page "Code")

## Explanation

Kent is a solo musician and wanted a website to share with fans and as a promotional tool for future bookings. This website was built using AngularJS, HTML5, SASS(CSS3) with Bootstrap, the Firebase API and Grunt.

## Use Case + Solution

User Story      | Implementation
------------- | -------------
As a user, I want to view and update a list of upcoming shows  | Create a button with the ngClick directive to trigger a function that starts/resets the timer. Use an ngBind directive to handle the button text. Use Angular's $interval service to execute a function that updates the remaining time every second.
As a user, I want to listen to songs | Create a boolean variable to control the state of the timer. Use the ngShow or ngHide directive to determine what the user sees in the view. When the timer reaches the end of a work session, modify it so the user will see this new time, and the ngShow or ngHide directive used on the buttons will pair the correct button to the timer's state.
As a user, I want to view and update a song-list  | Create a variable that holds the number of completed work sessions. Increment the count after each completed work session. When the timer reaches the end of a work session, update the time remaining by using a conditional statement to check whether the number of completed work sessions is equal to four - which would then send you to a thirty minute break. Once all sessions are complete, reset back to 0.
As a user, I want to view photos | Assign the time remaining to a variable and use {{ }} markup or the ngBind directive to render the time remaining in the view. Create a filter to handle the conversion of the time remaining.

<!-- ## Results

Bacon ipsum dolor amet filet mignon meatball spare ribs fatback bacon shankle. Kielbasa andouille fatback salami, boudin bresaola pig alcatra turkey spare ribs jerky. Corned beef bresaola leberkas salami alcatra beef landjaeger venison shank bacon meatloaf beef ribs picanha. Leberkas sausage brisket porchetta shankle prosciutto chicken picanha kielbasa pig kevin t-bone turducken filet mignon jowl. -->


