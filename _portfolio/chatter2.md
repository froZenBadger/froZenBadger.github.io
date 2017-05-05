---
layout: post
title: Chatter
thumbnail-path: "img/chatter.png"
short-description: Chatter is a messaging app for communicating with family, friends, and colleagues in real time.

---

{:.center}
![]({{ site.baseurl }}/img/chatter.png)

## Explanation
With chatter I was looking to explore one way of creating a real time messaging app. Chatter is built with AngularJS as well as Firebase for the backend database. Leveraging angularFire as well was about all else that was formed the foundation for the project.

## Problem
* How to require users to login, we did not want to authorize anonymous posting
* How to store and send messages as well as make communication occur in real time
* We needed to store different chat rooms to organize the communication flow as well as allow users to create chat rooms
* Allow users to create persistent accounts

## Wireframes
{:.center}
![]({{ site.baseurl }}/img/list-chat-rooms.png)
{:.center}
![]({{ site.baseurl }}/img/new-chatroom-btn.png)
{:.center}
![]({{ site.baseurl }}/img/new-chatroom-modal.png)
{:.center}
![]({{ site.baseurl }}/img/list-messages.png)
{:.center}
![]({{ site.baseurl }}/img/set-username-modal.png)
{:.center}
![]({{ site.baseurl }}/img/send-messages.png)

## Solution
* Creating the Firebase database on the backened was crucial to this project, specifically setting up the database design to be de-nested as possible allows for less tree traversal and mitigates otherwise potential pitfalls. In de-nesting db foreign id's were assigned ultimately creating an organized relational database
* To allow users abiltiy to create chat rooms the bootstrap modal was leveraged. 
* Similarly a modal was leverage for the setting of the username. In addition storing uername info in cookies allowed for the req'ment of a username to be present before allowed access to app. 
* Building on these was the AngularFire Auth API allowing users to store acounts with the app, which in turn allowed for a contact list to be stored. 
* The real time feature is fully fucntional due to the CRUD features of the database

## Results
Consistent results have provided support for a successful app

## Conclusion
The state of the app is stable and we are pleased with the results, yet I am  continuing to improve on the app. Features to be on the look out for include but are not limited to: 
* Creating admin users
* Allowing users to create private chat rooms
* Allow users ability to see who in their contact list is online
* Allow users ability to know when their active correspondent is typing  
Coming soon!