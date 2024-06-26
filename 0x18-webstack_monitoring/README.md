tack monitoring
=========================

DevOpsSysAdminmonitoring

*   Weight: 1
*   Project over - took place from May 8, 2024 6:00 AM to May 9, 2024 6:00 AM
*   An auto review will be launched at the deadline

#### In a nutshell…

*   **Auto QA review:** 0.0/12 mandatory
*   **Altogether:**  **0.0%**
    *   Mandatory: 0.0%
    *   Optional: no optional tasks

### Concepts

_For this project, we expect you to look at these concepts:_

*   [Monitoring](/concepts/13)
*   [Server](/concepts/67)

![](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/281/hb3pAsO.png)

Background Context
------------------

“You cannot fix or improve what you cannot measure” is a famous saying in the Tech industry. In the age of the data-ism, monitoring how our Software systems are doing is an important thing. In this project, we will implement one of many tools to measure what is going on our servers.

Web stack monitoring can be broken down into 2 categories:

*   Application monitoring: getting data about your running software and making sure it is behaving as expected
*   Server monitoring: getting data about your virtual or physical server and making sure they are not overloaded (could be CPU, memory, disk or network overload)

![](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/281/ktCXnhE.jpg)

Resources
---------

**Read or watch**:

*   [What is server monitoring](/rltoken/km_XUDAfXEBoXZQsIWEo5Q "What is server monitoring")
*   [What is application monitoring](/rltoken/z9jsikINjrsUo2QY5_Xz8g "What is application monitoring")
*   [System monitoring by Google](/rltoken/_8KIbIUNzMgKi_LiGMBWAw "System monitoring by Google")
*   [Nginx logging and monitoring](/rltoken/V3GsrDcMHPdgrizShj4RCg "Nginx logging and monitoring")

Learning Objectives
-------------------

At the end of this project, you are expected to be able to [explain to anyone](/rltoken/Bd9r8twsVT3S_8j7-kOLrg "explain to anyone"), **without the help of Google**:

### General

*   Why is monitoring needed
*   What are the 2 main area of monitoring
*   What are access logs for a web server (such as Nginx)
*   What are error logs for a web server (such as Nginx)

### Copyright - Plagiarism

*   You are tasked to come up with solutions for the tasks below yourself to meet with the above learning objectives.
*   You will not be able to meet the objectives of this or any following project by copying and pasting someone else’s work.
*   You are not allowed to publish any content of this project.
*   Any form of plagiarism is strictly forbidden and will result in removal from the program.

Requirements
------------

### General

*   Allowed editors: `vi`, `vim`, `emacs`
*   All your files will be interpreted on Ubuntu 16.04 LTS
*   All your files should end with a new line
*   A `README.md` file, at the root of the folder of the project, is mandatory
*   All your Bash script files must be executable
*   Your Bash script must pass `Shellcheck` (version `0.3.7`) without any error
*   The first line of all your Bash scripts should be exactly `#!/usr/bin/env bash`
*   The second line of all your Bash scripts should be a comment explaining what is the script doing

Your servers
------------

Name

Username

IP

State

98484-web-01

`ubuntu`

`35.174.184.115`

running

Actions Toggle Dropdown

*   [Soft reboot](/servers/77033/soft_reboot)
*   [Hard reboot](/servers/77033/hard_reboot)

*   [Ask a new server](/servers/77033/ask_new)

98484-web-02

`ubuntu`

`54.173.83.6`

running

Actions Toggle Dropdown

*   [Soft reboot](/servers/77027/soft_reboot)
*   [Hard reboot](/servers/77027/hard_reboot)

*   [Ask a new server](/servers/77027/ask_new)

98484-lb-01

`ubuntu`

`54.144.131.64`

running

Actions Toggle Dropdown

*   [Soft reboot](/servers/77028/soft_reboot)
*   [Hard reboot](/servers/77028/hard_reboot)

*   [Ask a new server](/servers/77028/ask_new)

Tasks
-----

### 0\. Sign up for Datadog and install datadog-agent

mandatory

Score: 0.0% (Checks completed: 0.0%)

For this task head to [https://www.datadoghq.com/](/rltoken/Ufs6rTHMET5LB1Uoylx0nw "https://www.datadoghq.com/") and sign up for a free `Datadog` account. When signing up, you’ll have the option of selecting statistics from your current stack that `Datadog` can monitor for you. Once you have an account set up, follow the instructions given on the website to install the `Datadog` agent.

![](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2019/6/6b0ea6345a6375437845.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240512%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240512T224239Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=c54581afe4325096736f20217175c055df093aab2bfe71c515e53581226c8642)

*   Sign up for Datadog - **Please make sure you are using the US website of Datagog (https://app.datadoghq.com)**
*   Use the **US1** region
*   Install `datadog-agent` on `web-01`
*   Create an `application key`
*   Copy-paste in your Intranet user profile ([here](/rltoken/elXu5CcaGpeK7GxerBb7wQ "here")) your DataDog `API key` and your DataDog `application key`.
*   Your server `web-01` should be visible in Datadog under the host name `XX-web-01`
    *   You can validate it by using this [API](/rltoken/5BtVPmgzhb96y7jZDGGHOQ "API")
    *   If needed, you will need to update the hostname of your server

**Repo:**

*   GitHub repository: `alx-system_engineering-devops`
*   Directory: `0x18-webstack_monitoring`

Done?! Check your code

×

#### Correction of "0. Sign up for Datadog and install datadog-agent"

Start a new test Close

Requirement success

Requirement fail

Code success

Code fail

Efficiency success

Efficiency fail

Text answer success

Text answer fail

Skipped - Previous check failed

Ask for a new correction : in progress... : an error occurred Get a sandbox QA Review

×

#### 0\. Sign up for Datadog and install datadog-agent

##### Commit used:

*   **User:** \---
*   **URL:** Click here
*   **ID:** `---`
*   **Author:** \---
*   **Subject:** _\---_
*   **Date:** \---

### 1\. Monitor some metrics

mandatory

Score: 0.0% (Checks completed: 0.0%)

Among the litany of data your monitoring service can report to you are system metrics. You can use these metrics to determine statistics such as reads/writes per second, which can help your company determine if/how they should scale. Set up some `monitors` within the `Datadog` dashboard to monitor and alert you of a few. You can read about the various system metrics that you can monitor here: [System Check](/rltoken/4RPOEVDTqKXuvyU4Gkj2Bw "System Check").

![](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2019/6/6a4551974aadc181e97a.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240512%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240512T224239Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=1f8338a8929794aee7c9a996901f0669cf497b3aa20c68a39f95d7d06b9495a3)

*   Set up a monitor that checks the number of read requests issued to the device per second.
*   Set up a monitor that checks the number of write requests issued to the device per second.

**Repo:**

*   GitHub repository: `alx-system_engineering-devops`
*   Directory: `0x18-webstack_monitoring`

Done?! Check your code

×

#### Correction of "1. Monitor some metrics"

Start a new test Close

Requirement success

Requirement fail

Code success

Code fail

Efficiency success

Efficiency fail

Text answer success

Text answer fail

Skipped - Previous check failed

Ask for a new correction : in progress... : an error occurred Get a sandbox QA Review

×

#### 1\. Monitor some metrics

##### Commit used:

*   **User:** \---
*   **URL:** Click here
*   **ID:** `---`
*   **Author:** \---
*   **Subject:** _\---_
*   **Date:** \---

### 2\. Create a dashboard

mandatory

Score: 0.0% (Checks completed: 0.0%)

Now create a dashboard with different metrics displayed in order to get a few different visualizations.

*   Create a new `dashboard`
*   Add at least 4 `widgets` to your dashboard. They can be of any type and monitor whatever you’d like
*   Create the answer file `2-setup_datadog` which has the `dashboard_id` on the first line. **Note**: in order to get the id of your dashboard, you may need to use [Datadog’s API](/rltoken/n2KPoJtwzx8LjCpmCB4KVQ "Datadog's API")

**Repo:**

*   GitHub repository: `alx-system_engineering-devops`
*   Directory: `0x18-webstack_monitoring`
*   File: `2-setup_datadog`

Done?! Check your code

×

#### Correction of "2. Create a dashboard"

Start a new test Close

Requirement success

Requirement fail

Code success

Code fail

Efficiency success

Efficiency fail

Text answer success

Text answer fail

Skipped - Previous check failed

Ask for a new correction : in progress... : an error occurred Get a sandbox QA Review

×

#### 2\. Create a dashboard

##### Commit used:

*   **User:** \---
*   **URL:** Click here
*   **ID:** `---`
*   **Author:** \---
*   **Subject:** _\---_
*   **Date:** \---

×

#### Recommended Sandboxes

Running only

### 2 images(0/2 Sandboxes spawned)

### Ubuntu 16.04

Basic Ubuntu 16.04 with vim, emacs, git and curl

Run

### Ubuntu 16.04 - Python 3.5 / Fabric / Puppet

Ubuntu 16.04 with Python 3.5, Fabric and Puppet installed

Run
