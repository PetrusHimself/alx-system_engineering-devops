0x0C. Web server
================

DevOpsSysAdmin

*   Weight: 1
*   Project will start Mar 25, 2024 6:00 AM, must end by Mar 27, 2024 6:00 AM
*   Checker will be released at Mar 25, 2024 6:00 PM
*   An auto review will be launched at the deadline

![](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/266/8Gu52Qv.png)

Background Context
------------------

[![](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/266/Screenshot+2017-07-06+19.24.05.png)](https://www.youtube.com/watch?v=AZg4uJkEa-4&feature=youtu.be&hd=1)

In this project, some of the tasks will be graded on 2 aspects:

1.  Is your `web-01` server configured according to requirements
2.  Does your answer file contain a Bash script that automatically performs commands to configure an Ubuntu machine to fit requirements (meaning without any human intervention)

For example, if I need to create a file `/tmp/test` containing the string `hello world` and modify the configuration of Nginx to listen on port `8080` instead of `80`, I can use `emacs` on my server to create the file and to modify the Nginx configuration file `/etc/nginx/sites-enabled/default`.

But my answer file would contain:

    sylvain@ubuntu cat 88-script_example
    #!/usr/bin/env bash
    # Configuring a server with specification XYZ
    echo hello world > /tmp/test
    sed -i 's/80/8080/g' /etc/nginx/sites-enabled/default
    sylvain@ubuntu
    

As you can tell, I am not using `emacs` to perform the task in my answer file. This exercise is aiming at training you on automating your work. If you can automate tasks that you do manually, you can then automate yourself out of repetitive tasks and focus your energy on something more interesting. For an [SRE](/rltoken/9I0WufjKdW3TZA2EVrGnlQ "SRE"), that comes very handy when there are hundreds or thousands of servers to manage, the work cannot be only done manually. Note that the checker will execute your script as the `root` user, you do not need to use the `sudo` command.

A good Software Engineer is a [lazy Software Engineer](/rltoken/sRY__axKNHhNW0SVmsUC_A "lazy Software Engineer"). ![](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/266/82VsYEC.jpg)

Tips: to test your answer Bash script, feel free to reproduce the checker environment:

*   start a `Ubuntu 16.04` sandbox
*   run your script on it
*   see how it behaves

Resources
---------

**Read or watch**:

*   [How the web works](/rltoken/6TI3HiyFdwrbXWKVF24Gxw "How the web works")
*   [Nginx](/rltoken/vkVMGlaf39j2DWAQWzo6EA "Nginx")
*   [How to Configure Nginx](/rltoken/zKrpVxWuUHVdW4URAjdFbw "How to Configure Nginx")
*   [Child process concept page](/rltoken/Ar18u5sRis1fkvkVgzdcqg "Child process concept page")
*   [Root and sub domain](/rltoken/xi3peVqYl02PfpHHHlCtxQ "Root and sub domain")
*   [HTTP requests](/rltoken/sBrrP4EAmI3NoYjIgZrUhw "HTTP requests")
*   [HTTP redirection](/rltoken/Eaa4ZuKvye941hTkP8VlBQ "HTTP redirection")
*   [Not found HTTP response code](/rltoken/eJSp2QFTY6jqqNtz8OVDEw "Not found HTTP response code")
*   [Logs files on Linux](/rltoken/7WMNY5CWD-CBrxmQrdmfPg "Logs files on Linux")

**For reference:**

*   [RFC 7231 (HTTP/1.1)](/rltoken/BGa6RrS0dnM6EdBGS_ZDUw "RFC 7231 (HTTP/1.1)")
*   [RFC 7540 (HTTP/2)](/rltoken/IZ2fyYn1qNZ9RXXsg5vG1g "RFC 7540 (HTTP/2)")

**man or help**:

*   `scp`
*   `curl`

Learning Objectives
-------------------

At the end of this project, you are expected to be able to [explain to anyone](/rltoken/EHyxcIwPtD2SzEGRKOnT3g "explain to anyone"), **without the help of Google**:

### General

*   What is the main role of a web server
*   What is a child process
*   Why web servers usually have a parent process and child processes
*   What are the main HTTP requests

### DNS

*   What DNS stands for
*   What is DNS main role

### DNS Record Types

*   `A`
*   `CNAME`
*   `TXT`
*   `MX`

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
*   You can’t use `systemctl` for restarting a process

