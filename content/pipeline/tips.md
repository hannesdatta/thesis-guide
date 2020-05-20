---
title: "Tips to structure your code"
draft: false
date: 2020-05-14T09:00:00+02:00
weight: 20
---

- Each source code file you are writing typically has *inputs* (e.g., a raw data set), carries out *some operations* (e.g., cleaning), and then saves its *outputs*.

- When working with R, your workspace gets easily cluttered and you may reach memory limits quickly. Also for other software packages, you may encounter memory issues. Therefore, we advise you to *split your project into smaller, independent code chunks*, all of which have *inputs*, *some operations* ("stuff to do in the code"), and *outputs* (e.g., temporary files, final data files).
    - For example, have three separate code files that (a) load the data, (b) clean it, and (c) analyze it.
    - Tie these code chunks together using `makefiles`.
    - When running into memory issues when prototyping your code, close and restart R, and then only load the required source code file.
