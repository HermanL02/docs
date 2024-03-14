---
title: Task Structure
description: A Koii task executable is a single JavaScript file that contains all of the functions for a Koii task to function properly.
image: img/thumbnail.png
sidebar_label: Task Structure
---

# Task Structure

The Koii [task template](https://github.com/koii-network/task-template) contains three separate JavaScript files that contain all of the functions for a Koii task to function properly.


```javascript
📦K2-TASK-TEMPLATE
 ┣ 📂_koiiNode
 ┃ ┗ 📜koiiNode.js // Contain all the components that task connect to K2.
 ┣ 📂task
 ┃ ┣ 📜index.js // Main file that contains the task function.
 ┃ ┣ 📜submission.js // Contains the task function and submitTask function.
 ┃ ┣ 📜audit.js // Contains the auditTask function.
 ┃ ┗ 📜distribution.js // Contains the submitDistributionList and auditDistribution function.
 ┣ 📂tests
 ┣ 📜config-task.yml
 ┣ 📜coreLogic.js
 ┗ 📜index.js

 ```

The task function, audit function, and distribution function were mentioned in the previous section; you can find `task/submission.js`, `task/audit.js`, and `task/distribution.js` in the task template that contains the functions for each of these steps.

:::tip
Confused on how task runs? Check out the [Runtime Flow](/concepts/what-are-tasks/what-are-tasks/runtime-flow) to understand the task execution flow.
:::

Next, we will go through each of these functions in detail.
- [Execute Task](/develop/write-a-koii-task/task-development-guide/task-structure/execute-task)
- [Audit Submissions](/develop/write-a-koii-task/task-development-guide/task-structure/audit-submissions)
- [Distribute Rewards](/develop/write-a-koii-task/task-development-guide/task-structure/distribute-rewards)