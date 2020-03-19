---
title: "The Art of YAGNI"
date: 2020-03-15T21:38:21-05:00
feature_image: "/img/woman-holding-face-mask.jpg"
author: "Jacob Ouellette"
tags: ["concept"]
---

The year is 2020, the world is been ravaged by the worst air-borne, alcoholically named, viral disease modern man has ever known! 

<!--more-->

**THE CORONAVIRUS.**

**DUN DUN DUUUUUUN!!!!!**

Ok that was a bit dramatic, but in all seriousness, you'd think the world was coming to an end with all the people rushing out to walmart and buying every. single. roll. of toilet paper. I went on an ice cream run yesterday night, and it was mind blowing to see a walmart in the heart of Dallas look like everyone was preparing for a category 5 hurricane. Toilet paper, paper towels, napkins, and any other paper product that could possibly be used to clean yourself up after you've finished your business was picked clean. The shelves looked like a scene from any zombie/apocalypse movie. 

![Do not cross](/img/crime-scene.jpg)

The scene of people stacking products in their cart like tetris pieces reminded me of a very useful concept I use at work on a daily basis, even if I'm not explicitly reminding myself to use it. This my friends is YAGNI. An idea in which every developer from any industry using any language should be aware of, understand, and use.

## The Actual Information

Let's get down to business (to defeat the Huns) and really discuss YAGNI. What does it stand for? Why should I, as a software engineer, care? How do I apply this amazingly fantastic and not at all abstract rule? Well I'll be answering all of those questions and hopefully any other needy questions I know that us engineers ask. So sit down, open up your favorite note taking application and let's do this!

To put it simply, YAGNI stands for "You Ain't Gonna Need It" (preferably spoken in a southern drawl). So if that reminded you of exactly what it is and how to use it, you can stop reading; However, if you're still unaware of how that applies to software development don't worry. I'm going to be discussing how I apply it to my work daily.

The idea of YAGNI is that as developers, we should only develop software as we need it. If developers didn't use YAGNI, software would never make it to production, be sold, and make money which means we would all be unemployed. I have worked with many software engineers who want to build a feature that will satisfy the customer's request, but also be customizable enough for another customer, oh and it will remind you to pick up milk on the way home, and they will want it to... You get the idea. As developers we want to build the world's greatest piece of technology, but that piece of software will never actually be finished. There is no end goal.

![Don't Be this guy](/img/man-using-macbook.jpg)

In comes the savior of the day, YAGNI. We effectively solve the problem above by only working on the features/bugs that users or business people want us to do. If a customer requests a feature, we should plan out the feature to fulfill that customer's request. If a bug report comes in, the code committed relating to that bug should only fix that bug. 

I have personally made commits that rewrite entire methods, because it had a single off by one error, but I knew it could be written in a more efficient way. This all seems fine and dandy, except that I wasted a bunch of time rewriting the method to save 12ms off the request time. Guess how many customers knew that there was an improvement on that endpoint and were thankful that someone put their time and effort into it. If you said 0, you are the winner! Come on down to be our next contestant on 'Rhetorical Questions'!

Since I decided to completely rewrite the method that was causing the problem I had a fun filled day of writing the code, followed by a couple of hours responding to PR comments, and then finally getting the changes merged into a release branch. If I had followed the rule of YAGNI I could have solved the issue in the existing code in about 15 minutes, PR approved in about 5 minutes, and the branch merged into a release in less than an hour from when I actually started working on the bug.

I forgot the rule of YAGNI and it cost me an entire day of development. So now you may be asking yourself, "How can I apply YAGNI to my specific situation". I have come up with a few steps to follow and/or ask yourself when deciding if something is worth delving into and fixing properly or if we can put on our navy seal hat, get in, do our job, and get out.

## The 4 Steps of YAGNI
### 1. Have the Request Written Out

This will usually be done by your managers and the business people who actually interact with the customers. It comes to engineers in the form of a ticket for us to discuss at a weekly meeting like sprint backlog grooming or something similar. This is where developers should ask clarifying questions about the ticket. As a developer we should also start getting a rough estimate of what the solution is going to look like.

### 2. Investigating the Solution

I have most commonly seen this time called a "Spike". Which is a set amount of time for developers to look into a ticket discussed at a backlog grooming session to figure out what actually needs to be done to fix the ticket. Take this time to figure out how to solve the bug/implement the feature into existing code. This is also when I take notes about code that is starting to get dated, doesn't follow the current code standards, or anything that seems odd.

### 3. Making the Plan (The Hard Part)

This is where YAGNI really starts to kick in. We need to go over all of the notes we made in the previous step and figure out what you need and what "you ain't gonna need". When implementing a new feature this step is a bit easier, because as developers we generally don't have an understanding of exactly what the user wants so we can go off of what the ticket says to do. For fixing bugs this step is very important. If the bug is simple to fix and there are no major changes that need to be made I suggest you just fix the issue and move on. The code was already working properly and if you need to come back to it, you can. It will still be there.

### 4. Execute

It's your time to shine! Get those fingers moving. Make the keyboard clack. Do whatever it is you deemed necessary to complete the ticket.

![This can be you!](/img/man-wearing-white-suit-jacket-and-white-pants.jpg)

Using the steps outlined above I've been able to smash my way through more tickets than I was in the past. I don't spend nearly as much time refactoring old code to get minor improvements or to meet the team's current code standards (which are going to change in a year or two anyway). Best of all, our users are happier, because the features and bug fixes are coming out faster. 

Now it's your turn. Go out there and implement YAGNI. At first it will be tough to understand what is truly necessary and what is additional fluff, but over time you'll become a YAGNI expert. It may also be useful when you're first starting out to go back on some recent tickets you've completed and run through the process of YAGNI as if you were doing those tickets again from scratch. You know what they say, "Hindsight is 20/20". So we can use this hindsight to improve our understanding of YAGNI and how to implement it in the future!
