---
layout: essay
type: essay
title: "We Must Enforce Coding Standards"
# All dates must be YYYY-MM-DD format!
date: 2025-02-13
published: true
labels:
  - Coding standards
  - Programming
  - EsLint
---
<img width="600px" class="rounded float-start pe-4" src="../img/headerimage.jpg">
Having standards, no matter if it’s regarding a profession or a hobby, allows for one to dedicate more time to focusing on the doing rather than fixing. What I mean is this, would you rather be able to complete a task and have it done in such a way that its context is easily understood by the layman who may 
come by and view it, or would it be preferable to have to come back and change things around to fit a new piece of information in to provide more context. The former is surely better than the latter. This holds especially true for those who program for a living. Having coding standards greatly reduces the chance 
that you’ll have to go back and refactor old code and helps the next programmer understand what is going on.

## To Be Explicitly Clear
When thinking about writing a new program, you should be explicitly clear from the get-go about what its functions do and how it interlaces with (possibly) existing code. One way to do this is to use code indentation, clear variable and function names that do exactly as they are named, and separation of long 
parameter inputs. You wouldn’t want someone who is working with your old code to have to restart a project because they misread a line of code, right? Save yourself and your colleagues from headaches and be sure to use a coding standard, whether it be a workplace standard or something common such as ESLint.

## Code Readability V.s. Efficiency 
Balancing code readability and efficiency is a key challenge in software development. Readable code, with clear variable names/functions, proper indentation, and easy-to-read design, ensures maintainability. However, sometimes performance optimizations require more complex implementations, such as reducing loops 
and minimizing memory usage. While clean code is easier to debug and extend, highly optimized code can be cryptic and harder to maintain. The key is to strike a balance; and prioritize readability unless performance is a bottleneck. When optimizations are necessary, document the reasoning behind them. Following 
best practices like refactoring, modularization, and leveraging built-in language efficiencies ensures code remains both efficient and easy to understand, reducing long-term technical debt and developmental issues.
Technical Debt
Technical debt accumulates when developers prioritize speed over code quality, often due to tight deadlines or lack of coding standards. Over time, poorly structured code becomes harder to maintain, leading to bugs, inefficiencies, and increased development costs. By following coding standards, teams can minimize 
technical debt, making sure that code remains readable and more importantly, scalable. Refactoring, or systematically improving existing code without altering its functionality, is essential for managing debt. Regular code reviews, automated testing, and documentation help prevent debt from spiraling out of control. 
Using standardized code upfront saves time and resources, reducing long-term project risks.

## EsLint
Earlier I mentioned EsLint as a common coding standard that could be used. In my ICS 314 class - Software Engineering, we recently started implementing this coding standard into our class WODs and I can say that it has been a game changer for me. The EsLint extension in Visual Studio Code forces you to conform 
to a specific standard by treating a break of coding standards as equivalent to a syntax error and shows an error in your code, forcing you to fix it. Humans by nature are adaptive creatures and when faced with a problem, we learn to adapt and overcome it. I’ve noticed that even after a few sessions of using EsLint, 
I automatically write my code using this new standard without having to be corrected by the IDE. Pair that with the fact that I’m still learning Typescript, it is forcing my brain to use the same part of my brain that learns language syntax. Very cool!


## Conclusion
In the end, following a coding standard is not just about writing cleaner code; but about improving efficiency and long-term maintainability. Whether through tools like ESLint, making readable code, or managing technical debt, consistency in programming will certainly be helpful in all of these areas. 
By prioritizing clear, structured code from the start, developers like you and I can focus more on the doing rather than fixing! In a field where changes are inevitable, embracing standards ensures smoother workflows and better software development.
