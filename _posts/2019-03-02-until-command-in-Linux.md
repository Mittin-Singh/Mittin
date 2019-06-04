---
layout: post
title: 'Until Command in Linux '
date: 2019-03-02
excerpt: Until Command in Linux.
tags:
  - Linux
  - Commands
comments: true
published: true
---
# Linux Until Command

<center>![](../img/until.png)<center>
<br>

until command in Linux used to execute a set of commands as long as the final command in the ‘until’ Commands has an exit status which is not zero. It is mostly used where the user needs to execute a set of commands until a condition is true.

### Syntax:
        until COMMANDS; do COMMANDS; done

Here, if the COMMANDS get evaluated to false then the statements will be executed. If the COMMANDS get evaluated to true then the no statements will be executed and control will go after the done statement.

### Example:

![](../img/until-example.png)


# Thanks !!!

## Furthermore, if you have any query, feel free to ask in the comment section.
