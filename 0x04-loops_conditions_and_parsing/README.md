0x04. Loops, conditions and parsing
===================================

DevOpsShellBashScripting

*   Weight: 1
*   Project over - took place from Jan 25, 2024 6:00 AM to Jan 26, 2024 6:00 AM
*   An auto review will be launched at the deadline

#### In a nutshell…

*   **Auto QA review:** 0.0/83 mandatory & 0.0/30 optional
*   **Altogether:**  **0.0%**
    *   Mandatory: 0.0%
    *   Optional: 0.0%
    *   Calculation:  0.0% + (0.0% \* 0.0%)  == **0.0%**

About Bash projects
-------------------

Unless stated, all your projects will be auto-corrected with Ubuntu 20.04 LTS.

Background Context
------------------

[![](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2019/6/b07e3333b1edfb9beed5.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240325%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240325T084716Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=782cbb44164845905680f99e435f997601b3844df8f566f99317ffd8462491f6)](https://youtu.be/BC2neyc5GcI)

Resources
---------

**Read or watch**:

*   [Loops sample](/rltoken/wT98UJfv_E2tk4yP9PcLLw "The <code>for</code> loop" target=“_blank”>The <code>for</code> loop</a> </li>
    <li><a href=")
*   [Variable assignment and arithmetic](/rltoken/olvOKX699pq50rkHRE5cSA "Variable assignment and arithmetic")
*   [Comparison operators](/rltoken/HxohzllkOWh0t4dy_HptIQ "Comparison operators")
*   [File test operators](/rltoken/g8of2ABPEJfCNtPrDQaqVw "File test operators")
*   [Make your scripts portable](/rltoken/O0Ay21p7tDhfLMsYbtAKug "Make your scripts portable")

**man or help**:

*   `env`
*   `cut`
*   `for`
*   `while`
*   `until`
*   `if`

Learning Objectives
-------------------

At the end of this project, you are expected to be able to [explain to anyone](/rltoken/UnkzDNdH09TFJ0-Y56azyg "explain to anyone"), **without the help of Google**:

### General

*   How to create SSH keys
*   What is the advantage of using `#!/usr/bin/env bash` over `#!/bin/bash`
*   How to use `while`, `until` and `for` loops
*   How to use `if`, `else`, `elif` and `case` condition statements
*   How to use the `cut` command
*   What are files and other comparison operators, and how to use them

Requirements
------------

### General

*   Allowed editors: `vi`, `vim`, `emacs`
*   All your files will be interpreted on Ubuntu 20.04 LTS
*   All your files should end with a new line
*   A `README.md` file, at the root of the folder of the project, is mandatory
*   All your Bash script files must be executable
*   You are not allowed to use `awk`
*   Your Bash script must pass `Shellcheck` (version `0.7.0`) without any error
*   The first line of all your Bash scripts should be exactly `#!/usr/bin/env bash`
*   The second line of all your Bash scripts should be a comment explaining what is the script doing

### Copyright - Plagiarism

*   You are tasked to come up with solutions for the tasks below yourself to meet with the above learning objectives.
*   You will not be able to meet the objectives of this or any following project by copying and pasting someone else’s work.
*   You are not allowed to publish any content of this project.
*   Any form of plagiarism is strictly forbidden and will result in removal from the program.

More Info
---------

### Shellcheck

[Shellcheck](/rltoken/joK6l_yEZ9N7T0GQ1RDjLA "Shellcheck") is a tool that will help you write proper Bash scripts. It will make recommendations on your syntax and semantics and provide advice on edge cases that you might not have thought about. `Shellcheck` is your friend! **All your Bash scripts must pass `Shellcheck` without any error or you will not get any points on the task**.

`Shellcheck` is available on the school’s computers. If you want to use it on your own computer, here is how to [install it](/rltoken/jbz0_-i3TV3WpKgxhyrtpA "install it").

Examples:

Not passing `Shellcheck`:  
  
![](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/251/Vxotqyj.png)

Passing `Shellcheck`:  
  
![](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/251/ubHWxDU.png)

For every feedback, Shellcheck will provide a code that you can use to get more information about the issue, for example for code `SC2034`, you can browse [https://github.com/koalaman/shellcheck/wiki/SC2034](/rltoken/dxp49_rfO4_9Yjtcg59exg "https://github.com/koalaman/shellcheck/wiki/SC2034").

Tasks
-----

### 0\. Create a SSH RSA key pair

mandatory

Score: 0.0% (Checks completed: 0.0%)

Read for this task:

*   [Linux and Mac OS users](/rltoken/Cy1plV2eR3VphjPqliXB8A "Linux and Mac OS users")
*   [Windows users](/rltoken/074M_gTsD34x3Q6MX55PDw "Windows users")

man: `ssh-keygen`

You will soon have to manage your own **servers** concept page hosted on remote [data centers](/rltoken/nDPzEm5SYxcdGxP_OpVYXQ "data centers"). We need to set them up with your RSA public key so that you can access them via SSH.

Create a RSA key pair.

Requirements:

*   Share your **public key** in your answer file `0-RSA_public_key.pub`
*   Fill the `SSH public key` field of your [intranet profile](/rltoken/qsaEQ3ZWrgs-zoueDpXpPA "intranet profile") with the public key you just generated

