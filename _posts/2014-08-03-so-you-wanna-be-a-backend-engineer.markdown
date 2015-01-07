---
layout: post
title:  "So You Wanna be a Backend Engineer"
date:   2014-08-03
---

Below, you will find a continuation of the discussions that I am having with a computer science student at the University of South Florida. In this post, I have described what a backend engineer does and the sort of skills that should be learned to become a backend engineer. This article is the first in a series of articles that will dig into the concentrations of software engineers.

###The Job of a Backend Engineer
Backend engineers write the code that serves as the engine of an application. This code may be an application programming interface (API) to schedule an appointment, an email scheduler, or an algorithm to calculate a credit score. There are new libraries and frameworks appearing each month that may make a backend engineers job simpler. Much of the complexity in this job comes from determining whether or not it is worth the effort to implement these new solutions in your projects.

Pursuing the software development path of backend engineering may be for you if you are fascinated by the classic algorithms you’re taught in school, you enjoy learning about obscure data structures, or if you’re always looking for the most efficient way to solve a problem. For many (including myself), this is what makes programming so exciting.

###Pick a Language
There are many questions out there about which language is the best. When it comes to backend engineering, you’ll often see Python, Java, and C# as “the best language.” My recommendation: choose one and learn everything you can about it. Java and Python are platform independent and often deployed on *nix while C# is a must if you’re going to be working in a .Net environment. Every language has a core set of features and then common libraries that extend the language. It’s important to know both, but libraries can be learned much more quickly when you know the core of the language.

There are two key pieces to learning the core language. One, you need to read the docs. This can be done either through the online documentation created by the programming language maintainers or by finding books that teach the language. In my experience, books are good at teaching the basics while the online docs allow you to dig into the minutiae. Two, try out a diverse set of projects to allow you to use as many packages as possible. These projects can be fifty lines of code to complete a discrete task or they can stretch across multiple files in order to integrate several concepts to solve a problem. I will suggest some projects later on.

In all cases, I believe you should store your projects in Github. This will not only give you a central location for all of your past work, but also a repository of code that you can present to interviewers when applying for a job.

###Always Work on Problem Solving
This is a common theme across all types of software engineering. We can always get better at problem solving and should always do everything in our power to improve ourselves in this area. The key here is to think through each problem we have to solve. I like talking through problems with my peers to gain new perspective and to find deficiencies in my logic.

[Project Euler][project euler] provides a great set of problems that require you to think critically. With many of these problems, using a brute force method will take too much time, forcing you to create more efficient solutions. By pushing yourself through these exercises, you will look at problems presented to you in a different way.

###Build on Top of Databases
It’s possible to build applications by writing any information to text files and reading from those files when the application is restarted. When you get into more robust programs, following this design is difficult and (usually) a poor choice. However, using a database is not enough. You should spend time learning about relational data modeling. In many backend engineering roles, you will be responsible for building the data model. A good data model will make your job significantly easier.

For the purposes of learning, using an in-memory database like SQLite allows you to start working with a database quickly with minimal configuration. I like to use SQLite when getting started with a new project to allow myself to focus on the code rather than configuring a database. MySQL and PostgreSQL are popular open source databases that you can use to gain a deeper understanding of databases. A backend engineer must have a strong understanding of keys, indexes, and SQL.

###A Step-by-Step Guide
1. Choose a language and focus on it. Read the docs and learn the core language
2. Work on projects to improve your problem solving and gain more knowledge around your language.
3. Solve problems on [Project Euler][project euler] to improve critical thinking skills.
4. Spend time learning about databases. Data modeling, connectivity, etc.

###Suggested Projects
* A simple to-do list that stores the list in a database. This should require you to insert and read from the database.
* A web scraper that monitors a website for updates. Try doing this without a web scraping library for increased difficulty.
* A web services API that performs CRUD (create, read, update, delete) operations on a connected database.
* Implement a solution to the [dining philosopher’s problem][dining philosopher]. This is an advanced problem that requires knowledge of multithreading.

Of course, there’s much more to learn, but a lot of this learning depends on choices that you make as you work through these fundamental concepts.

**Shameless Plug:** LearnVest is looking for backend engineers of all skill levels! Check out our current backend engineering openings [here][hiring].

[project euler]: https://projecteuler.net/
[dining philosopher]: http://en.wikipedia.org/wiki/Dining_philosophers_problem
[hiring]: http://jobvite.com/m?3JeIAgw0