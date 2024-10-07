---
title: Event-based pipeline on the Web
tags: ["Production Management", "Database", "Web", "Fullstack", "Python", "Django", "Vue"]
date: 2022 - 2023
---

The [Flow](https://www.autodesk.com/ch-fr/products/flow-production-tracking/overview?term=1-YEAR&tab=subscription) production tracking software is home to a lot of manual changes by the user. It's a portal to every asset in the company and therefore can be used as an interface to trigger some automated work, for which I created a fullstack website using Django, Vue and Postgres.

Some of the responsibilities of this website was reacting to Webhooks sent by the Flow production tracking system on specific events. For example, the name of the animations were determined by a collection of metadata. So when a new animation is created by anyone in Flow then its name has to be updated accordingly.

The creation of an animation therefore triggers a Webhook to a URL on our website. The website then triggers an asynchronous task to rename the animation accordingly and stores the result of all of this in the database. A frontend lets us monitor all of this in realtime.
