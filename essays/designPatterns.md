---
layout: essay
type: essay
title: "Design Patterns and why they matter"
# All dates must be YYYY-MM-DD format!
date: 2025-04-15
published: true
labels:
  - Design Patterns
  - Software Engineering
---
<img width="1200px" class="rounded float-center pe-4" src="../img/project-estimation.png">
<br>
Take a look at any major modern city in the world today; they all have something in common: They are designed to make living among millions of other people possible. Tokyo, for example, has hundreds of thousands, if not more, different buildings all packed tightly together. It has train lines that operate on a tight 
schedule and can bring people from one half of the city to the other within an hour! How do you think this is done? Well, a group of people who are in charge of city planning must create a plan and a budget to allocate resources towards making the city livable and efficient. A blueprint of sorts. In a way, this is not
so different from creating a software project. 

## Why Do Design Patterns Matter?
Something we call "Design patterns" is what we implement to organize and implement readable and functional code. There are a myriad of different design pattern styles that one can follow, but the key is to be consistent throughout the design of your system. As the system
grows in complexity, so does the importance of having clean and easy-to-understand code. Furthermore, it allows you to encapsulate a solution to common problems in your system (i.e, think of needing to sort different types of arrays, just call a sort method which you have already implemented before). Design patterns serve
as an easy way to navigate your system's code base, like having a map in your pocket. It's less of a coding strategy and more of a blueprint for how to structure the code/files. 

## Design Pattern Strategies
As mentioned before, design patterns are meant to ease the burden of reading through complex code and to facilitate easier object creation and composition. The two main strategies are called creational patterns and structural patterns. Creational patterns help designers create objects in a flexible and reusable way.
An idea like building a customer's order step by step by combining a drink, a main, and a side is one way to understand this. You inherently know how to order a meal at McDonald's, even if you don't go often/ever, and this is sort of the same thing. Structural patterns are used to bring information under an umbrella of sorts.
Creating a file directory or system is certainly one way of defining structural patterns, but another way is to think of a component that can change an object dynamically without actually altering its structure.

## Examples of My Design Pattern implementations
In one of our WOD coding practices for my ICS 314 class, we had to implement a Jamba Juice store ordering system that took customer orders and tracked inventory. In this WOD, I used creational design patterns to take a customer's order using an object with many parameters and slowly developed code that built objects
to fit them, and eventually built up a customer's order from scratch. The inventory system used a form of structural design pattern called a decorator. This allowed me to dynamically update the inventory system without actually changing how it works or its overall structure. 

## Final Thoughts
Design patterns are an essential tool for creating software systems as they are the "blueprint" that helps keep everything not only in working order, but also comprehensible. Solutions to common problems can be marked, and a design can be implemented to easily solve problems that require them.  
They aren't just coding tricks but are foundational methods that help teams build scalable, readable, and maintainable code. Whether you're building a simple ordering system or a massive app, design patterns provide the architecture that turns spaghetti code into simple code review.

