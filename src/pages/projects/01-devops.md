---
title: Game Dev Space and DevOps
tags: ["CI", "CD", "Automation", "Docker", "Github Actions", "Infrastructure"]
date: 2022 - 2024
---

DevOps is a group of principles and practices that promotes monitoring, testing and automation of software development. It focuses on faster development cycles and software stability. It's about bridging the gap between Development (software creation) and Operations (managing and deploying the software).

In other words, DevOps is about setting up a toolchain that helps developers control their development cycle and the state of their software.

I started learning about Docker in 2022. While it's not a DevOps-specific tool, we can benefit a lot from it to replicate our software in consistent environments and automate tasks in said environments.

Having this new tool under my belt was key to develop and deploy the event-based website I made at [Quantic Dream](https://www.quanticdream.com/fr) in 2023. This let me control the environment of the website, share dependencies with coworkers, run tests and deploy easily.

It's when developing [Game Dev Space](https://game-dev.space/) that I really started setting up a whole DevOps pipeline dedicated to game development. Docker became essential to setup a variety of services on the cloud to setup automation based on Github Actions.

I would recommand the following GDC talk by Seth Coster on how Devops principles can be applied to game development: [Stress-Free Game Development: Powering Up Your Studio With DevOps](https://www.youtube.com/watch?v=t9HRzE7_2Xc).
