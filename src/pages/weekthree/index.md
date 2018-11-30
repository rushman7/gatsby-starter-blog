---
title: Sprint Challenge Week Three
date: "2018-11-30T22:40:32.169Z"
---
https://github.com/Lambda-School-Labs/Labs8-Cookbook/graphs/contributors - rushman7

## Weekly Question

This week has proven to be the toughest week for our group out of every week.
Up until know we were far and head of the curve of MVP requirements but now 
that it has come to functionality and putting everything together we really 
see the complexity of this project and data management that comes with it.
Unfortunately we did not manage to get everything functionally working yet,
roughly 80% is implemented and they others are still a work in progress. My
biggest challenge was working with a new stack with a not so steep learning
curve so it mostly involved reading documentation and slowly progressing from
there. Most of the implemented features include scraping data from two random
websites and then selecting the meal type and date to schedule for that recipe.
This creates an event that is then stored in the database. This even is linked
to a recipe which is then linked to a User so that only recipes related to the
use is shown. We've also implemented this data to be mapped out in our Recipes 
page which allows CRUD functionality on them. We also have this data show up
on our calendar with the corresponding date to the date selected. 

## Front End

* Day 1 Calendar API
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/43
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/56
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/58
  * https://trello.com/c/gEfR89m3/72-calendar-buttons

* Day 2 Buttons Component
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/46
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/47
  * https://trello.com/c/Dj9GNUOs/73-buttons-component

* Day 4 Calendar Visible Data
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/58
  * https://trello.com/c/FRIMLgeI/83-calendar-fe-be

## Back End

* Day 3 Prisma Query for Calendar
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/56
  * https://trello.com/c/FziNT0Vx/9-database-setup

* Day 1 Create Save Mutation
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/51
  * https://trello.com/c/gEfR89m3/72-calendar-buttons


## Calendar Visible Data:

Originally I was working with dummy data to have the calendar show data that
is passed from state. This was quickly changed with our gql query from our 
our back-end which now has access to that data that is stored by the user and
scraped from a website. The most challenging thing today was dealing the proper
syntax and ways of retrieving that data because our data was inside a nested
mutation. Access a nested mutation is extra challenging without the proper syntax.
Another challenge was refactoring the dummy data to match the proper name types
that we have given out 

## MVP 

* Deployed Front End: https://lambda-cookbook.netlify.com
* Deployed Back End: https://lambda-cookbook.herokuapp.com/

## Whiteboarding:

https://www.youtube.com/watch?v=LDWC3qDYYi0