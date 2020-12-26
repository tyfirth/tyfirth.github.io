---
layout: post
title:      "Christmas Panic or Unpermitted Parameters"
date:       2020-12-26 03:09:33 +0000
permalink:  christmas_panic_or_unpermitted_parameters
---

Unpermitted parameters, or problems with players

This last module has been extremely fun learning and the latest project has been very fun for the most part.  I have encountered a few road blocks throughout my application's development. At times I was cruising along and things were working fine, but there were a few instances that cost me hours of time.

Unpermitted parameters
My first major road block came when associating my players model with matches. Things seemed to be working ok until I attempted to create a new player along with a match using a .build method. I kept getting an error that told me the parameter players was not permitted, even though it was clearly written in my strong params for matches to permit players attributes. As usual, the fix was relatively simple but not before reading a hundred articles and going down another 100 dead ends. The players were not being permitted because they were not a hash as originally written. Enclosing the variable in curly braces seemed to do the trick and permitted the players attributes. 

Attempting devise
The next step was to set up authentication in the application. I had heard about a nice ruby gem called devise that was supposed to make authentication simple as long as you didn't need anything too fancy. Perfect for my needs, a simple authentication set up with a user to have a username and password, salted bcrypt password that integrates with the players model. i had never used devise before but the set up walkthroughs seemed simple and straightforward. After installing devise and setting up a user model to handle authentication, I attempted to associate it with the players model so a player belonged to a user and a user has one player. At this point everything stopped working and the more I tried to fix it the worse things got. After a few days of getting incremental improvements, I decided it would be best to go back to a point in my commits when things were working fine, before I added devise.

Branching with Github
I know the basics of GitHub and that's about it. I can make changes to a main branch and make commits to that branch from a remote origin. SO when I needed to go back, I hit my last major roadblock. You'd think it would be easy, and it probably is. But trying to work the bugs out of your rails project on Christmas Day when its due in a few hours leaves you feeling a little frantic and pressed for time.  I finally managed to figure out how to create a new branch and checkout a commit, but merging is still a little fuzzy. I'm not even sure I'll be adding the correct url when I submit my project tonight. 

I have everything working but its not on the main branch. I hope it all goes through ok.

These are all issues I should have run into a week ago. Live and learn. 

Although these speedbumps were aggravating beyond belief, struggling through them helped me understand what I was doing on a deeper level. I have learned a lot from each of these modules and while I do my best to change my strategy based on what I've learned, old habits tend to die hard. I'm learning it is extremely important to expect the unexpected, plan for the worst, and hope for the best. 

My new year's resolution is to be 2 - 3 weeks ahead for the remaining two modules.
