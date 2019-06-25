# Meesterproef 2019

## Table of Contents

1. [Introduction](#Introduction)
2. [Focus points](#Focus-points)
3. [Content](#Content)
4. [License](#License)

## Introduction

During the master test I worked on a project for [Wallscope](https://wallscope.co.uk/).
Wallscope is a company based in Edinburgh, Scotland.

I did this project together with three others: [Chelsea Doeleman](https://github.com/chelseadoeleman), [Jesper Ingels](https://github.com/jesperingels) and [Maikel Sleebos](https://github.com/Senpaizuri).
While working together we all tried to learn something new and fun. Some parts of design process had some overlap, but we each tried to scope our own pieces of the application. What that learning meant for me can be read later on.

During this 5 week period we created an experience which enabled medical students, medical researchers and reporters alike to work together on creating _digital cases_.
These digital cases were formed by searching the Wallscope datasystem, in an intuitive manner, and then group them together in one such case. A case can be a collaboration between multiple users of the system.
Wallscope gets this data from the [NHS](https://www.scot.nhs.uk/), which is the National Healthcare System of Scotland.

To provide the most use out of the system, we also decided not to restrict the basic search functionality behind an _account wall_. If you were to not be logged in, you simply wouldn't be able to participate in any of the _case_ related activities of the platform.

The project repository can be found [here](https://github.com/Maikxx/360-wallscope).

## Focus points

* **Web App From Scratch**
    * Structure the application modularly. ✅
    * Unit testing. ✅
    * Actor / Interaction / Data flow diagrams.
    * Refactoring ✅
    * _Nice to have_ -> end-to-end testing.
* **CSS To The Rescue**
    * Use [BEM](http://getbem.com/) and [SCSS](https://sass-lang.com/) to structure stylesheets. ✅
* **Browser Technologies**
    * _Nice to have_ -> Progressive enhancement with [Next.js](https://nextjs.org/).
* **Web design**
    * User tests
* **Performance Matters**
    * Create performing [PostgreSQL](https://www.postgresql.org/) queries. ✅
    * _Nice to have_ -> Minimize all outgoing files.
* **Real-Time Web**
    * Smart data management. [Redux](https://redux.js.org/)? Global state? Happy flow -> Client first, trace back in case of an error.

## Content

* [Process](./docs/PROCESS.md)
* [Design rational](./docs/DESIGN_RATIONAL.md)
* [Product biography](./docs/PRODUCT_BIOGRAPHY.md)
* [Reflection](./docs/REFLECTION.md)

## License

This repository is licensed as [MIT](LICENSE) by [Maikel van Veen](https://github.com/maikxx).