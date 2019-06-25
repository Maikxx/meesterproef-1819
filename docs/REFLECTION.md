# Reflection

## Web App From Scratch

When creating this application, I decided (in coordination with the rest of the group) to build the **boilerplate from scratch** (as in, not using create-react-app).

I set up the application with TypeScript, ReactJS, Express and PostgreSQL.
The goal of doing this, was to create a modular application that scales quite well.

Although I did have some experience creating boilerplates before, I had never built anything the scale of this project before, mainly regarding the server and database.

I came across a lot of hurdles and if I had to do this project again, I would have not started with creating all the "required" endpoints to get data from the server and instead would start to build it alongside the client. Because of time issues I had created endpoints, which we didn't use at all. This also meant a lot of features were missing.

Another thing that I would change is that I would only start to set up data models when I actually had received the data that would need to be in the system. I now had to guess a lot of the time and that guessing cost me a lot of time in the end. As Laurens said, only start working on something once you have received everything you need in order for the system to work.

I ended up also writing a few **unit tests** for some server functions. I found that I would need a lot more time to get these unit tests everywhere in the application and on the more difficult code functions. That's why I decided to not focus on this as much, instead focus on getting the application working in time. TypeScript is a good help for avoiding errors on the frontend as well. So that helps me justify the fact that I didn't go all the way in this topic.

When working together on such an application a lot of **refactoring** is also in place, meaning I had to do that a lot to create the most modular and reusable code for the case that Wallscope would go further with this current codebase.

I said **end-to-end testing** was a nice addition to the breakable nature of client-side rendered applications. That is exactly what it stayed as, a nice addition, since I didn't have time for this anymore. I do however, when I have energy for it again, want to take this one up, since it looks very valuable to me.

I wanted to originally also add the **actor, interaction and data flow diagrams** but seen the current situation that might or might not still be workable.

In summary, I think the most things that I learned during these few project weeks are regarding teamwork and how to structure things so that it is not only for me logical, but also for the other co-workers. The goal for me was not to learn a lot of new things, but rather help others learn a lot of new things.

I asked them if they felt helped by me at the times that I explained some new things to them and they said "yes". I do know, however, that I need to take a slower approach when explaining things. For me they are often very sensible, and then I explain them in the speed that I can work with them.

## CSS To The Rescue

Although I did not style a lot of the application myself during these past few weeks, I did convince everyone to use SCSS and BEM to structure the code.
This helped us all create code standards, so that they can be passed on to Wallscope if they wanted to have this code at all.
I like to think that I helped them learn another piece of new methodology, BEM, since most of them hadn't used this before.
Structuring code is always important, but especially when working with larger scale projects, where you work in collaboration with other developers.

## Browser Technologies

I added this goal as a nice to have to the learning goals. Because of a lack of time I didn't get to do this learning goal.
This means that there is barely any progressive enhancement in this application, since the client is rendered by React, which is not on the server. This means that in the case of JavaScript failing to load, there will be nothing shown to the page.
I would like to continue learning new ways to work with my favourite frontend framework of this time, in a progressively enhanced manner, when I have the time in the future.

## Web design

As a part of web design, we did a user test with a medical student. We tested mainly the design of the application, to check if there was something missing or something needed to be different.
We had some things that we needed to change in order for him to use it happily. Although this was not a goal I focussed on heavily, I felt like including it anyway, since I did in fact participate in the test and asked some questions which where important for the result of this test.

## Performance Matters

Creating a performing application was for me one of the most important learning goals, seeing as there was the most to be learned for me here.
You can take the basic performance optimizations, like including the compress package in the express configuration, however, I felt like the best way to increase performance in the application, was by writing good SQL queries, since SQL is way faster at handling getting data from multiple tables than doing the equivalent in JavaScript.
Before this project I had never worked with `join`s, which meant I tried to do all the logic SQL is actually best at in JavaScript, which made the queries very, very slow, since I had to merge multiple objects and arrays together.
I only scratched the surface of what's possible with SQL and performance in this language, for that matter.
I will definitely need more exercise doing this to be able to call myself somewhat skilled in working with SQL and performing queries.

## Real-Time Web

Although I did initially liked the focus of this goal the most, seeing as though I think the mentality of this way of writing code is way more enjoyable for the end user, I did not have the time to make this work.
I have read up some things about this happy flow coding pattern.
What I would have done if I had more time, is to create a centralized store on the client, where all data lives for the current user, so that the initial page load might take a little longer, but then all the following requests to the server are handled in the background, while the store is being updated synchronously. This results in a happy flow, where the user (ideally) never has to wait for responses from a server, which makes it look like everything works in a real-time way, while in fact it just stores things on the client immediately, while asynchronously sending the request to the server, only giving an error and tracing back when the server responses with something else than status 200.
Taking on this pattern is really interesting, since it also takes on the challenge of increasing perceived performance, which is part of the Performance Matters course.