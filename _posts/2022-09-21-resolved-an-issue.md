---
title: "resolved-an-issue"
date: 2022-09-21
---

I haven't visited the blog recently and have only been writing these files, but I'm writing this at 00:07, so let's just pretend that I wrote this on 9/21 :).

I started my bot up to try and start testing the commands out in my development server, but alas! The first command I tried (defer) wasn't working.
I distractedly tried to resolve this issue and was mislead by part of the stack trace.

I was being given some wording along the line of, "Message has already been replied to." so I thought, okay, maybe I'm calling the wrong command.
I tested several different things. Added a then/catch (is that how it's done in node.js?). Even looked at StackOverflow and other parts of the internet for the same error.
Long story short, I found nothing promising, and read different parts of the stack trace to where I found out my issue.
I removed the {} from around my require/import wait. That solved it! Apparently I need to learn when and why you use brackets around it. Or the proper call for if I do use brackets?

Tomorrow should be more fruitful in my endeavors.

- Tschüss!