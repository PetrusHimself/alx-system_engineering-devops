0x06. Regular expression
========================

RegexDevOps

*   Weight: 1
*   Project over - took place from Jan 30, 2024 6:00 AM to Jan 31, 2024 6:00 AM
*   An auto review will be launched at the deadline

#### In a nutshell…

*   **Auto QA review:** 0.0/24 mandatory & 0.0/9 optional
*   **Altogether:**  **0.0%**
    *   Mandatory: 0.0%
    *   Optional: 0.0%
    *   Calculation:  0.0% + (0.0% \* 0.0%)  == **0.0%**

Background Context
------------------

For this project, you have to build your regular expression using Oniguruma, a regular expression library that which is used by Ruby by default. Note that other regular expression libraries sometimes have different properties.

Because the focus of this exercise is to play with regular expressions (regex), here is the Ruby code that you should use, just replace the regexp part, meaning the code in between the `//`:

    sylvain@ubuntu$ cat example.rb
    #!/usr/bin/env ruby
    puts ARGV[0].scan(/127.0.0.[0-9]/).join
    sylvain@ubuntu$
    sylvain@ubuntu$ ./example.rb 127.0.0.2
    127.0.0.2
    sylvain@ubuntu$ ./example.rb 127.0.0.1
    127.0.0.1
    sylvain@ubuntu$ ./example.rb 127.0.0.a
    

Resources
---------

**Read or watch**:

*   [Regular expressions - basics](/rltoken/6VeaVMaugIxcFAwA27TBdQ "Regular expressions - basics")
*   [Regular expressions - advanced](/rltoken/rntjh3-3S86zt0Qy28L10w "Regular expressions - advanced")
*   [Rubular is your best friend](/rltoken/RGkVuw1lZ_hoCCbLsiOAhg "Rubular is your best friend")
*   [Use a regular expression against a problem: now you have 2 problems](/rltoken/Vwm8lpMUGa4x_FBtlyUQ8g "Use a regular expression against a problem: now you have 2 problems")
*   [Learn Regular Expressions with simple, interactive exercises](/rltoken/XsQ6rzS1uy-E6bnswUqIKg "Learn Regular Expressions with simple, interactive exercises")

Requirements
------------

### General

*   Allowed editors: `vi`, `vim`, `emacs`
*   All your files will be interpreted on Ubuntu 20.04 LTS
*   All your files should end with a new line
*   A `README.md` file, at the root of the folder of the project, is mandatory
*   All your Bash script files must be executable
*   The first line of all your Bash scripts should be exactly `#!/usr/bin/env ruby`
*   All your regex must be built for the Oniguruma library

### Quiz questions

**Great!** You've completed the quiz successfully! Keep going! (Show quiz)

#### Question #0

What is the `/school/` regexp matching?

*   school
    
*   School
    
*   schoOl
    

#### Question #1

What is the `/Scho*l/` regexp matching?

*   Schoo.l
    
*   Scho.l
    
*   Schoool
    

#### Question #2

