---
title: Sprint Challenge Week Four
date: "2018-12-07T22:40:32.169Z"
---
https://github.com/Lambda-School-Labs/Labs8-Cookbook/graphs/contributors - rushman7

## Weekly Question

Styling seems to be quite the separation in terms of coding between
team-mates. Everyone has their own taste of styling and it showed
in our group this week because we had multiple cases where our css
was overwritten because it did not reflect the team's overall goal.
To circumvent this, we had our own custom mockups created to facilitate
our overall direction for the project in terms of styling and this
drastically helped us maintain a common theme amongst the group and 
throughout the entire project. We've all rotated this week in terms
of getting the functionality polished as well as making the front-end
look presentable, my primary focus this week was getting the calendar
to display data as well as modify data. After this, moving into styling
the calendar. 

* Documentation:
  * https://lambda-cookbook.netlify.com/home 
    We need to add some content about our entire project on the home page
  * https://lambda-cookbook.netlify.com/home/recipes
    We need to fix a cropping issue with images in our Recipes cards
  * https://lambda-cookbook.netlify.com/home/calendar
    More detailed styling needed for the calendar
  * https://lambda-cookbook.netlify.com/
    A more intuitive landing page

## Front End

* Day 1 Calendar API
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/65
  * https://trello.com/c/UnTOhWR0/90-fix-calendar-and-add-clickablility

* Day 2 Portal Component
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/65
  * https://trello.com/c/CpfbGd7g/93-portal-calendar-portal

* Day 4 Search Bar + Settings Page CSS
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/76
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/78
  * https://trello.com/c/dPNbV4Yp/103-search-box-and-settings-page

## Back End

* Day 3 Portal Mutation
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/73
  * https://trello.com/c/lBzvrTLt/100-portal-modal-mutation



## Portal Mutation:

Now that we have data persisting throughout the calendar it was time
to create a modal to modify both the meal type and date of each event.
This was achieved through reacts V.16 new feature; Portal's. Portal's
allow a user to create a modal, a separate instance of react completely
and work with a brand new component rather than rerouting them. Within
this brand new separate instance i passed mutations from graphQL in order
to modify the data on the back-end and persist it on our screen without 
the need to re-render or re-load the data.

## MVP 

* Deployed Front End: https://lambda-cookbook.netlify.com
* Deployed Back End: https://lambda-cookbook.herokuapp.com/

## White-boarding:

https://www.youtube.com/watch?v=LDWC3qDYYi0