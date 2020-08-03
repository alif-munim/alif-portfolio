---
title: What is Containerization?
id: what-is-containerization
category: development
tags: [reactjs, javascript, typescript, html, css ]
date: 2020-08-01T05:25:44.226Z
path: blog/what-is-containerization
cover: ./preview.png
excerpt: Learning docker, kubernetes, and other containerization technologies.
---

I recently came across a video of the [GitHub Arctic Code Vault](https://www.youtube.com/watch?v=fzI9FNjXQ0o) located in the frigid Norweigan tundra.
The vault, constructed from a decomissioned coalmine, is right next to the Svalbard global seed vault and will house all of the world's open-source code safely for the next 1,000 years. As I watched, awestruck by the beauty of Svalbard and the thought that my javascript tic-tac-toe game will be preserved for the enjoyment of generations to come, I came across one comment that still has me cracking up a week later.

<br/><br/>
!["Imagine how many tapes will be wasted on people who didn't gitignore node_modules..."](./comment.PNG)
<br/><br/>

Though it was an amusing thought, the reason the comment stuck with me was a little different. For the modern JavaScript developer, the `node_modules` folder is rarely even a passing thought. It eats away at a large portion of a project's memory, and is conventionally ignored when pushing to GitHub as it can be restored with a simple `npm install` command. It holds an assortment of packages, dependencies, and code written by thousands of other developers that form the foundation of our own creations.

Today, the fabric of the world is formed by code. It is an intricate network of tools that are all tightly woven and highly interdependent. One missing package, broken tool, or unsupported version number can bring an entire system to a crashing halt. Intensifying these issues is the fact that physical machines often differ vastly from one end-user to the next, adding even more variability to an already chaotic system. This is where containerization comes in.

<br/><br/>
![A comparison of containerization and virtual machines](./docker-containerization.png)
<br/><br/>

Containerization is the practice of encapsulating software and all of its dependencies into a single package that runs consistently across all systems regardless of operating systems or physical architecture. Traditionally, the same result was achieved through virtual machines which required a hypervisor and each with their own guest operating systems which ran on a host machine. However, containerization offers a lightweight alternative as multiple containers can share a single OS kernel and run isolated from all other system processes inside of a containerization engine. Furthermore, this means that apps can be modularized through the containerization of their functional components and the orchestration of these containers inside of a network.

In my next blog post, I'll explore Docker and Kubernetes, the de-facto standard tools for building, sharing, and running containerized applications everywhere from local machines to the cloud.


<br/><br/>