---
layout: essay
type: essay
title: "Sweet Solutions: Cookie Cutter Code Patterns"
# All dates must be YYYY-MM-DD format!
date: 2023-04-24
published: true
labels:
  - Design Patterns
---

## To Cookies or Not To Cookie

<img width="300px" class="rounded float-start pe-4" src="../img/cookie.png">

In the realm of software development, we often find ourselves in a digital kitchen, mixing ingredients to create delectable programs that meet specific requirements. Picture yourself in a kitchen, about to bake a batch of digital cookies for a project. You have a variety of cookie cutters at your disposal, each designed to create a specific shape with precision and ease. Just as these cookie cutters save time and energy by eliminating the need to handcraft each cookie, design patterns streamline the coding process, allowing us to craft consistent, high-quality products with minimal effort. They act as the "cookie cutters" of the coding world, each tailored for a specific purpose, enabling developers to create efficient, maintainable, and flexible code with ease.

Of course, while design patterns are an invaluable resources for streamlining the coding process, it's unrealistic to expect to write professional-level code with just design patterns alone. Having a vast collection of cookie cutters may seem impressive, but it's impossible to make every cookie shape imaginable with just the available cutters. Cookie cutters serve as templates, limiting what can be produced, much like design patterns. While design patterns can inspire solutions, they're not a one-size-fits-all solution, and simply utilizing a design pattern doesn't automatically mean the most efficient code possible. Therefore, developers must balance the use of design patterns with creativity and innovation to find the best possible solutions for each unique problem.

## Design Patterns in practice  

As a beginner in software engineering, I have found that almost every programming problem I encounter has already been addressed, and there is usually an established design pattern available to solve it. This especially the case with the current project I'm working on as my team and I are developing an application that helps users discover clubs at the University of Hawaii Manoa that align with their personal interests. An issue that we had was that we needed a way of maintaining a data collection that dynamically updates the client side and some way of making only parts of said data collection available, depending on its use case such as bookmarking clubs. A key component and major design pattern that we utilized for this was the Publish-Subscribe pattern; A fundamental design pattern in Meteor. The Publish-Subscribe pattern allowed us to establish clear communication between the data sources, or publishers, and the event bus that relays new state changes to the appropriate subscribers. With this pattern, we were able to ensure that only the necessary parts of the data collection were made available to each subscriber.

Overall, design patterns are a valuable tool for software engineers, offering time-tested "cookie cutter" solutions to recurring problems. By leveraging these patterns, we can create code in a more efficient manner as we no longer have to spend the time to make everything from scratch. As I continue to grow in my software engineering journey, I look forward to discovering new and exciting design patterns to incorporate into my projects.
