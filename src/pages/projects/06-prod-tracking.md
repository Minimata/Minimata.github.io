---
title: Architecturing production tracking
tags: ["Python", "Automation", "Production Management"]
date: 2019 - 2024
---

At [Quantic Dream](https://www.quanticdream.com/fr), the tool used for production tracking is called [Flow](https://www.autodesk.com/ch-fr/products/flow-production-tracking/overview?term=1-YEAR&tab=subscription) (previously Shotgun, then Shotgrid). It's basically Excel sheets on steroids, on the cloud, structured like a database. This is where people go to look at the production status of certain assets, their upward and downward dependencies, etc.

All of these assets have to be structured together as so called entities. The entities and their relationships are key to have a meaningful representation of the assets and their metadata. I've been in charge of this structure for my five years at Quantic Dream.

Flow also has an API to be able to access its data through code. This API is quite barebones and non-opinionated so I made a python wrapper around it. This was used around most of our python toolchain when needing to interact with Flow in a way that fit our workflows better through a single library which helped for debugging.
