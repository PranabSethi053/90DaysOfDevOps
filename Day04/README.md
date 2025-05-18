*) What is Kernel?

    The kernel is a computer program that is the core of a computer’s operating system, with complete 
    control over everything in the system.

*) What is Shell?

    A shell is a special user program that provides an interface for users to interact with operating 
    system services. It accepts human-readable commands from users and converts them into instructions
    that the kernel can understand. The shell is a command language interpreter that executes commands
    read from input devices such as keyboards or from files. It starts when the user logs in or opens a    terminal.

*) What is Linux Shell Scripting?

    Linux shell scripting involves writing programs (scripts) that can be run by a Linux shell, such as    bash (Bourne Again Shell). These scripts automate tasks, perform system administration tasks, and 
    facilitate the interaction between users and the operating system.

*) Explain in your own words and with examples what Shell Scripting means for DevOps.

    All those shell commands which we apply to do some work can be also fit into a particular format,
    means with proper syntactic and semantic approach. Through this we can automate some task rather 
    than doing that manually. So this process can be known as Shell Scripting.
    
    (Example) Environment Setup:
    #!/bin/bash
    apt update && apt install -y nginx git docker.io
    systemctl enable nginx

*) What is #!/bin/bash? Can we write #!/bin/sh as well?

    This is called a shebang (or hashbang). It's used at the top of a script to tell the system which 
    interpreter to use to run the script.

    #! is a special character sequence.
    /bin/bash is the path to the Bash shell.
    
    Yes, we can use #!/bin/sh instead of #!/bin/bash, but there are differences:

    #!/bin/sh refers to the standard system shell, which is usually a link to another shell (like dash
    on Ubuntu or bash in POSIX compatibility mode).

    Scripts with #!/bin/sh are expected to follow POSIX-compliant syntax.
    bash has extra features not available in sh (e.g., arrays, [[ conditional expressions, brace 
    expansion).

*) Write a Shell Script that prints I will complete #90DaysOfDevOps challenge.
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ vim devops_challenge.sh

    #!/bin/bash   
    echo "I will complete #90DaysOfDevOps challenge."

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ chmod +x devops_challenge.sh

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ./devops_challenge.sh
    
    I will complete #90DaysOfDevOps challenge.

*) Write a Shell Script that takes user input, input from arguments, and prints the variables.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ vim input_example.sh

    #!/bin/bash

    # Take user input
    read -p "Enter your name: " name

    # Read from command-line arguments
    arg1=$1
    arg2=$2

    # Print the values
    echo "Hello, $name!"
    echo "First argument: $arg1"
    echo "Second argument: $arg2"

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ chmod +x input_example.sh

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ./input_example.sh DevOps Linux
    Enter your name: Pranab Sethi
    Hello, Pranab Sethi!
    First argument: DevOps
    Second argument: Linux

*) Provide an example of an If-Else statement in Shell Scripting by comparing two numbers.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ vim compare_numbers.sh
    
    #!/bin/bash

    # Read two numbers from the user
    read -p "Enter first number: " num1
    read -p "Enter second number: " num2
    
    # Compare the numbers
    if [ "$num1" -gt "$num2" ]; then
      echo "$num1 is greater than $num2"
    elif [ "$num1" -lt "$num2" ]; then
      echo "$num1 is less than $num2"
    else
      echo "Both numbers are equal"
    fi
    
     HP@PRANAB MINGW64 /c/Pranab (main)
     $ chmod +x compare_numbers.sh

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ./compare_numbers.sh
    Enter first number: -5
    Enter second number: -9
    -5 is greater than -9
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ./compare_numbers.sh
    Enter first number: 9
    Enter second number: 9
    Both numbers are equal
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ./compare_numbers.sh
    Enter first number: 0
    Enter second number: 8
    0 is less than 8
