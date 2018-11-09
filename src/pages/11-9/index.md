---
title: Sprint Challenge Week One
date: "2018-11-09T22:40:32.169Z"
---
https://github.com/Lambda-School-Labs/Labs8-Cookbook/graphs/contributors - rushman7

## Weekly Question

This first week introduction to Labs has been an eye opener and a glimpse into
the professional developer life. I saw what it meant to work with a team of 
colleagues in a development environment and how challenging it can be to co-work
with people on projects that can easily break one-another. This week and for the
coming weeks my primary focus will be back-end web development. That stack our group
chose was React-Apollo(redux replacement)-GraphQL(Back-End)-Prisma(DB) with my 
primary focus being Prisma. One of the first biggest challenges i faced was for
obvious reason, learning Prisma. It's never easy learning a new development package
that you've never used before especially with the time crunch we have it was 
imperative that we have it up and running before the weekend. Fortunately we were
able to meet MVP expectations and go above and beyond this week with getting 
user authentication up and running via bcrypt and jwt on the back-end as well as
multiple well designed components on the front-end via React. I helped the team
solidify as a group with constant meeting's between everyone. On a daily bases out
of the 8 hours in the day we would all be in a zoom with one-another for a minimum
of 3 hours of that total time. My urge to progress forward and account for tasks 
that are not in our current goal-set is definitely something that can cause friction
in the group as it can easily delay our entire process to create a niche that i made.

## Front End

* Day 4 Header Component
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/18
  * https://trello.com/c/1TpcIHvo/40-header

## Back End

* Day 1 Prisma Setup
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/2
  * https://trello.com/c/FziNT0Vx/9-database-setup

* Day 2 Prisma Deploy
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/3
  * https://trello.com/c/xQmrGqhh/36-deploy-prisma-db-to-heroku

* Day 3 Prisma User Authentication and Query/Mutation
  * https://github.com/Lambda-School-Labs/Labs8-Cookbook/pull/10
  * https://trello.com/c/qDjIA90T/25-database-user-and-recipe-data-type

## Prisma User Authentication and Query/Mutation:

User Authentication wasn't necessarily difficult but rather lengthy in the process.
Our project deals with recipes that a user will save onto their account so our
current biggest hurdle is getting a way to have list data persist when a user is
authenticated. The work involved creating a type set for both User and Recipe which
has their own parameters. Prisma does a very good job at bidirectional relationships 
between set's so getting a recipe to persist on a user was no issue. ![user-data](https://trello-attachments.s3.amazonaws.com/5be072f2afaae80c3eb430d3/5be30d52c4c15f3022f181b8/a00c4b406b8ca0768cfe9952b5dcacef/a170325efe3a06203e3b467d6d644ec4.png)
In the image you can see that a recipe was successfully created name Spaghetti with the
proper parameters. At the bottom the "Authorization" value is coded with the users randomly
generated jwt. This confirms that the recipe was registered to the user. At the moment my
current issue is figuring out how to allow Prisma to retrieve the recipe data based on
the current user. This will take time in itself to create resolvers/functions for 
data retrieval. Another major bug that was run into and still has yet to be solved is
graphql automatic prisma post-deploy update. This means that when the `prisma deploy`
command is run in terminal it will update any changes we made to the database and graphql
has an integrated function that reads the Prisma data-model and automatically updates their
schema. ![post-deploy-error](https://trello-attachments.s3.amazonaws.com/5be072f2afaae80c3eb430d3/5be345cf59f374646837197a/0421757f69501963fe4ed5333197fc0f/c8bc4f23d25772654faf1d1fcc9f81d0.png) 
The error has persisted through every possible fix that 
google-fu had to offer and it still remains today, however there is a fairly simple 
work-around to this was to manually enter the graphql command in terminal:
`graphql get-schema --project prisma`. I also made my relational type sets such as
"ingredient-recipe" and "ingredients" but left those commented out until we get
the basics setup.


## MVP 

* Deployed Front End: lambda-cookbook.netlify.com
* Deployed Back End: https://lambda-cookbook.herokuapp.com/