# Product Biography

## Table of Contents

* [Design Brief & Planning](#Design-Brief-&-Planning)
    * [Design Brief](#Design-Brief)
    * [Planning](#Planning)
* [Research & Inspiration](#Research-&-Inspiration)
* [Ideas & Insights](#Ideas-&-Insights)
* [Product Development](#Product-Development)

## Design Brief & Planning

### Design Brief

### Objectives & Goals

Initially the client (Wallscope) wanted to have effectively a redesign of the NHS website.
From the start, I thought this was a really boring task, which killed all my motivation to work on this project.
When we as a group contacted Joost about this, he also confirmed this feeling.
Then we had to call with Wallscope to confirm our new idea.

### Planning

| Date(s)           | Activity                                                                   |
|-------------------|----------------------------------------------------------------------------|
| Every monday      | Call with Wallscope about the progress                                     |
| Every friday      | Project coaching                                                           |
| 22-5-19           | Research provided case data                                                |
| 27-5-19           | Project briefing at AUAS                                                   |
| 29-5-19 / 1-6-19  | Concept inspiration visit to Edinburgh, Scotland, including design research |
| 3-6-19 / 4-6-19   | Finalize concept mock-ups                                                   |
| 5-6-19 / 7-6-19   | Set-up development boilerplate                                              |
| 10-6-19 / 22-6-19 | Development on the product                                                 |
| 24-6-19 / 26-9-19 | Documentation                                                              |
| 27-9-19           | Deadline                                                                   |

To view the changes (which there are a lot of) to the planning, please refer to [the process file](./PROCESS.md).

## Research & Inspiration

Before even starting the project, I started to research the case a little bit more, with the data Wallscope provided to us.

The first article I read was about [triple stores](https://medium.com/wallscope/linked-data-a-conceptual-exploration-9860a1f44d68?source=friends_link&sk=a4a70e4b3af9326157a0386981a0a84f). After reading this article from them it kind of made sense, but still kind of didn't, because I didn't see the benefit of using this over joined SQL tables with described relations.
After taking some time to take this information in, it started to make sense, seeing as the relations are set in the data explicitly, instead of implicitly, which can (on large scale applications), save a lot of time thinking about relations.

During the first few days of the project, we all took upon ourselves to find inspirational interfaces which could be meaningful to us.
We mainly started to look at inspiration for _dashboards_ and _native mobile applications_, as well as _infographics_, _charts_, _graphs_ and _data visualizations_.

As a team we created a shared [Pinterest board](https://nl.pinterest.com/chelsea_doelema/wallscope-web-dev/) to store our inspiration research in, on which I also participated to search for inspiration.

We also received some of their current visualizations, which I felt like definitely needed improvement, due to the fact that they may or may not convey meaning, but look like crap.

* [Prescribed medicines](https://www.isdscotland.org/Health-Topics/Prescribing-and-Medicines/Publications/2019-05-14/visualisation.asp)
* [A&E Waiting times](https://www.isdscotland.org/Health-Topics/Emergency-Care/Publications/2019-05-07/Summary/index.asp)
* [Mental health](https://www.isdscotland.org/Health-Topics/Mental-Health/Publications/2018-09-25/psychiatric-inpatient-activity/?28376406432)

As a team, we also did an interview with a medical student in week 4.
I wasn't the interview leader, but came up with a few smart questions for the person on the fly. For example, since we created designs in a so called **dark mode** (mainly because of my own personal feelings towards **non-dark mode** interfaces), I asked him if he would rather use a **light mode** over a dark mode.
This question came up to me, because he said that he worked barely late at night, which is when dark modes are most often used.
He felt the interfaces color scheme was a little too dark and depressing for working during the day, and would feel like having the light mode by default over the dark mode.

For further detail on the interview and what other things came from it, please refer to [this document](https://github.com/Maikxx/360-wallscope/blob/master/docs/USER_TEST.md).

As a learning goal that I set for myself, I wanted to learn something about unit testing (in Node applications specifically).

Here is what I found, and used as a basis to write my [article about unit testing](https://github.com/Maikxx/weekly-nerd-1819/blob/master/articles/UNIT_TESTING.md):

* [https://www.tsmean.com/articles/how-to-write-a-typescript-library/unit-testing/]()
* [https://journal.artfuldev.com/unit-testing-node-applications-with-typescript-using-mocha-and-chai-384ef05f32b2?gi=cb0aac915670]()
* [https://medium.com/@RupaniChirag/writing-unit-tests-in-typescript-d4719b8a0a40]()
* [https://wanago.io/2019/02/04/typescript-express-testing/]()
* [https://wanago.io/2019/02/04/typescript-express-testing/]()
* [https://mochajs.org/]()
* [https://www.chaijs.com/]()

## Ideas & Insights

From researching **unit testing** applications with TypeScript, Mocha and Chai, I learned that this is a whole new can of worms to open.
I found it to be very difficult to combine my personal goal to learn a bit about unit testing with the development of the project, which is why I didn't go very far in depth.
When I did a unit test on some piece of code I took for granted though, it did break, twice. Once because of a typo, and the other time because it was just bad code.
This lead me to forget the fact to take everything for granted. I could really see the use in unit testing after this, although creating fake mocks and integrating tests in the code with database calls provided to be way too difficult.

After performing the **user test**, though, I got reminded to the fact that no one human is alike, and that my personal thoughts didn't overlap with a potential users thoughts.
This was very much the truth in the case of the **dark mode** of the application.
I always have every application that has a dark mode, switched to dark mode, always. So after testing, it appeared that this application was not really the right place for a dark mode (at least for that users context).

## Product Development

Although I did personally not sketch a lot of things during this project, I did keep a [process document](./PROCESS.md) up-to-date and also created a [simple design](https://github.com/Maikxx/360-wallscope/blob/master/docs/BRIEFING_3.md).

Also, to take a look at what particular things I worked on in this project, feel free to take a look here, at the [GitHub project](https://github.com/Maikxx/360-wallscope/projects/1), where we all assigned tasks to ourselves to take on.

To view the final application, [click here](https://wallscope.herokuapp.com).