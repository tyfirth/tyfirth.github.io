---
layout: post
title:      "React-Redux Project"
date:       2021-04-29 20:21:27 -0400
permalink:  react-redux_project
---


First draft of blog:

My first blog was all about getting stuck and being persistent until you're unstuck. I'm stuck. 

I've learned to start simple and add complexity as needed, but even though I started simple, React Redux isn't simple. I'm having a hard time understanding a few redux concepts and how to put them into practice. Most of the blogs I've searched share similar sentiments, that React-Redux isn't easy to grasp for newcommers. I definitely agree. Further, many of the examples from the labs don't encapsulate what I'm trying to accomplish with my particular project. 

Simply put, I don't know what I don't know. 

Update:

Well, after many hours of headaches and debugging, the application finally works. Best of all, I think I actually know what I'm doing now with React-Redux! Wow! I think my biggest hang up was the information flow from components to action creators to the reducer! The reducer is where it's at! I had to be much more careful and considerate of the state i was wanting to get back, and what specific information was actually beging sent to my database. Luckily I got some good help that untangled some of my incorrect thoughts about how everything was put together. Additionally, I hit a snag where everything was rendering except for my recipe show page. What solved that? Well, I believe its that the component I wanted the recipe page to render ON was a child of the component it was actually rendering on. So to fix it, all I needed to do was bring the recipe page route up one level to the home container so that it was a sibling of the recipe container component it was ultimately being rendered to. React Redux is definitely not user friendly for beginners like myself. But now that I feel I have a better handle on the logic, I'm excited to start my next, and first, personal project!
