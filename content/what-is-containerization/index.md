---
title: What is Containerization?
tags: [reactjs, javascript, typescript, html, css ]
date: 2020-08-01T05:25:44.226Z
path: blog/what-is-containerization
cover: ./preview.png
excerpt: Learning docker, kubernetes, and other containerization technologies.
---

I recently came across a video of the [GitHub Arctic Code Vault](https://www.youtube.com/watch?v=fzI9FNjXQ0o) located in the frigid Norweigan tundra.
The vault, constructed from a decomissioned coalmine, is right next to the Svalbard global seed vault and now houses all of the world's open-source code safely for the next 1,000 years. As I watched, awestruck by the beauty of Svalbard and the thought that my javascript tic-tac-toe game will be preserved for the enjoyment of generations to come, I came across one comment that still has me cracking up a week later.

<br/><br/>
<img src="./comment.PNG" width="200"/>
<br/><br/>

Though it was a very amusing thought, the reason the comment stuck with me was a little different. Even for those of us who have worked with Node, the `node_modules` folder is rarely even a passing thought. It eats away at a large portion of a project's memory, and is conventionally ignored when pushing to GitHub as it can be restored with a simple `npm install` command. It holds all of the other packages, dependencies, and code written by thousands of other developers that our own projects rely on. 

<br/><br/>