---
title: Sprint Challenge Week Two
date: "2018-11-16T22:40:32.169Z"
---

## Weekly Contribution

https://github.com/Lambda-School-Labs/Labs8-Cookbook/graphs/contributors - rushman7

## Weekly Question

The first week went so smoothly for us that i felt as if we were invincible going into
this project. The second week could not have hit us any harder and seriously woke us
up to what it truly means to be in professional development environment. This week was 
not easy, we had many errors upon many errors pile up at the seems in what looked like
a never ending rabbit hole. Fortunately we hit our MVP goals through everything but 
much like any battlefield, wounds remain. One of our biggest issues was organization
between our github. It was a daunting task trying to make sure that everyone is on board
and on the same page about every single change we make. Implementing the Pages and API's
*for now* was not too big of an issue, however most of these pages do not have
functionality yet so next week will come the test of time for us. My primary focus this
week was connecting our frontend to our backend and in that regard i was successful. 
Our frontend interfaces with our bank and data is displayed in the Recipes page i created
for said reason. Other than connecting my pieces have not integrated with other groupmates
yet, however that time will come. All in all, this week was brutal for us but in the end
we made it to our MVP goal and will continue to push forward. 

## Front End

* Day 2 Calendar Component + Google API (WIP)
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/28
  * https://trello.com/c/rOI5Jy5x/52-front-end-apollo-configuration-and-recipe-data-calendar-component-api* 

* Day 3 Recipes Component
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/33
  * https://trello.com/c/R6GrciFg/64-recipes-component

## Back End

* Day 1 Apollo Integration connecting FE + BE
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/24
  * https://trello.com/c/7iEdwt2s/46-connect-front-end-to-back-end-with-apollo

## Components + Google API:

I though i would have the least amount of struggles when tackling React Components
this week which was pleasantly the case. React always seems to save me in my time 
of need however it wasn't all roses and rainbows. I was able to successfully implement
our backend data and have it passed as props. I turned them all into Note Cards similiar
to our project design(WIP). All recipes shown are from our backend.![recipes](https://i.gyazo.com/7a0542ae30abd535fc85f05145023288.png) 
Our issue now is data retrieval from our deployed backend server which will require us to 
implement cors on the deployed server, a task for next week. I added minimal styling to 
the Recipes Component as our current focus is having our functionality down. The second
component is actually an API, a Calendar API. This one was fairly easy to implement 
however there is an issue between our css code and css-loader/style-loader so the css
for the calendar is not properly being loaded. Another task we will have to sort out in
the coming weeks. ![calendar](https://trello-attachments.s3.amazonaws.com/5be072f2afaae80c3eb430d3/5bec56484ffc9847f2a4ba86/ed7ec30a554278ab09905367872b6e5f/d6a6139e3d49c41dff73db48c6b77b15.png) 


**Integer Pairs Whiteboarding**
https://www.youtube.com/watch?v=fu6yf0YT_BE

## MVP 

**Front and Back End Servers Connected:** 
Front end can view recipes from our database
https://lambda-cookbook.netlify.com/home/recipes

**Users Can Create Accounts:** 
https://cookbookproject.auth0.com/login?state=g6Fo2SBTUFFDNTkyMVgxUkE1NDNjSUdYcjlmWWZkQTh5UEZYX6N0aWTZMmdhRm8yU0J2TmtRNVZtWlBibFZKUmtsSldFUlRPRmQwY25oMGFsOU9jemxWUkRoMlJBo2NpZNkgN2tsVzFUdEphZXM3WnJla3FOWGF2Ykpyd1dRTGtEZjA&client=7klW1TtJaes7ZrekqNXavbJrwWQLkDf0&protocol=oauth2&response_type=token%20id_token&redirect_uri=https%3A%2F%2Flambda-cookbook.netlify.com%2Fcallback&scope=openid&nonce=fM7CuYcgqBAGneRIC4ELpccIbvXwKXl~&auth0Client=eyJuYW1lIjoiYXV0aDAuanMiLCJ2ZXJzaW9uIjoiOS44LjIifQ%3D%3D

**APIs and Services Working:** 
https://lambda-cookbook.netlify.com/home/settings
https://lambda-cookbook.netlify.com/home/calendar