---
description: The control center of your Naas server.
---

# ⚡ Naas manager

The “⚡️ → Production folder” visible in your file system is where you can see where your notebooks and files are sent to be scheduled, exposed, triggered to create data products.

## Concept

Going to production should not be so complicated.

Today, you need to :

* Deploy a server
* Setup a cron job
* Ask some technical help to maintain it in the long run

With Naas, everything is setup. You just need to manage a **Production folder.**

## How it works ?

When you run Naas magic low code formulas (see the **Features section**), your notebook is automatically sent to the "⚡️→ Production" folder.

![](<.gitbook/assets/Screenshot 2022-01-05 at 23.20.04.png>)

Here will be kept:

* Your latest notebook
* Your files dependencies
* Your history of each notebook with a timestamp
* The output notebook (in case you need to debug, you will see here the error message)