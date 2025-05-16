*) If you noticed that there are a total of 90 sub-directories in the directory '2023' of this repository, what did you think? How   did I create 90 directories? Manually one by one, using a script, or a command?

    All 90 directories were created within seconds using a simple command:

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ mkdir day{1..90}
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ls
     2024_GIT_TUTORIAL/                  day69/
     90DaysOfDevOps/                     day7/
    '90DaysOfDevOps(LondheSubham153)'/   day70/
     ansible_playbook                    day71/
     ansible_roles                       day72/
     ansible-inventory                   day73/
    'bhai document.pdf'                  day74/
    'CIC-IOT(Attacks).pdf'               day75/
     connecting-instances/               day76/
     Cryptography1.zip                   day77/
     day1/                               day78/
     day10/                              day79/
     day11/                              day8/
     day12/                              day80/
     day13/                              day81/
     day14/                              day82/
     day15/                              day83/
     day16/                              day84/
     day17/                              day85/
     day18/                              day86/
     day19/                              day87/
     day2/                               day88/
     day20/                              day89/
     day21/                              day9/
     day22/                              day90/
     day23/                             'DevOps & CloudComputing'/
     day24/                              docker_volume
     day25/                              Dockerfile-multi-stage
     day26/                              Exam_Folder/
     day27/                              Git/
     day28/                              HTML/
     day29/                             'IMPETUS GURUKUL (OLD COURSE)'/
     day3/                               JAVA/
     day30/                              kuberentes_notes_app
     day31/                              Lec-13.ppt
     day32/                              Lec-14.ppt
     day33/                              Lec-15.ppt
     day34/                             'math linear algebra'/
     day35/                              metal/
     day36/                              Movies/
     day37/                              MyFolder1/
     day38/                              MyFolder2/
     day39/                              MyProject/
     day4/                               newfolder/
     day40/                             'Nimcet Documents'/
     day41/                              node-cicd
     day42/                              open_source
     day43/                             'Original Documents'/
     day44/                              Photo.jpg
     day45/                              photos/
     day46/                              Pranab
     day47/                              Prolog/
     day48/                              prometheus_grafana
     day49/                             'Python(Jupiter)'/
     day5/                               Python_Data-Types_Assignment.ipynb
     day50/                              README.md
     day51/                              Sample-Github-Actions-Workflow/
     day52/                              ShellScripts/
     day53/                              Software/
     day54/                              Springboot_bankapp_Kubernetes
     day55/                              terraform_ec2
     day56/                              terraform_EC2_Data_Variable_Output
     day57/                             'thermo lecture 10'/
     day58/                             'thermo lecture 11'/
     day59/                             'thermo lecture 12'/
     day6/                              'thermo lecture 13'/
     day60/                             'thermo lecture 14'/
     day61/                             'thermo lecture 15'/
     day62/                             'thermo lecture 16'/
     day63/                             'thermo lecture 5'/
     day64/                             'thermo lecture 8'/
     day65/                             'thermo lecture 9'/
     day66/                              Two-tier-Application
     day67/                              var/
     day68/


*) Create Directories Using Shell Script:

   Write a bash script createDirectories.sh that, when executed with three arguments (directory name, start number of directories, and end number of directories), creates a specified number of directories with 
   a dynamic directory name.
   Example 1: When executed as ./createDirectories.sh day 1 90, it creates 90 directories as day1 day2 day3 ... day90.
   Example 2: When executed as ./createDirectories.sh Movie 20 50, it creates 31 directories as Movie20 Movie21 Movie22 ... Movie50.


    HP@PRANAB MINGW64 /c/Pranab (main)
    $ vim createDirectories.sh
    
     #!/bin/bash
    
    prefix=$1
    start=$2
    end=$3
    
    for (( i=start; i<=end; i++ ))
    do
        mkdir "${prefix}${i}"
    done
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ chmod +x createDirectories.sh
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ./createDirectories.sh day 1 90
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ls
     2024_GIT_TUTORIAL/                  day45/   day90/
     90DaysOfDevOps/                     day46/  'DevOps & CloudComputing'/
    '90DaysOfDevOps(LondheSubham153)'/   day47/   docker_volume
     ansible_playbook                    day48/   Dockerfile-multi-stage
     ansible_roles                       day49/   Exam_Folder/
     ansible-inventory                   day5/    Git/
    'bhai document.pdf'                  day50/   HTML/
    'CIC-IOT(Attacks).pdf'               day51/  'IMPETUS GURUKUL (OLD COURSE)'/
     connecting-instances/               day52/   JAVA/
     createDirectories.sh*               day53/   kuberentes_notes_app
     Cryptography1.zip                   day54/   Lec-13.ppt
     day1/                               day55/   Lec-14.ppt
     day10/                              day56/   Lec-15.ppt
     day11/                              day57/  'math linear algebra'/
     day12/                              day58/   metal/
     day13/                              day59/   Movies/
     day14/                              day6/    MyFolder1/
     day15/                              day60/   MyFolder2/
     day16/                              day61/   MyProject/
     day17/                              day62/   newfolder/
     day18/                              day63/  'Nimcet Documents'/
     day19/                              day64/   node-cicd
     day2/                               day65/   open_source
     day20/                              day66/  'Original Documents'/
     day21/                              day67/   Photo.jpg
     day22/                              day68/   photos/
     day23/                              day69/   Pranab
     day24/                              day7/    Prolog/
     day25/                              day70/   prometheus_grafana
     day26/                              day71/  'Python(Jupiter)'/
     day27/                              day72/   Python_Data-Types_Assignment.ipynb
     day28/                              day73/   README.md
     day29/                              day74/   Sample-Github-Actions-Workflow/
     day3/                               day75/   ShellScripts/
     day30/                              day76/   Software/
     day31/                              day77/   Springboot_bankapp_Kubernetes
     day32/                              day78/   terraform_ec2
     day33/                              day79/   terraform_EC2_Data_Variable_Output
     day34/                              day8/   'thermo lecture 10'/
     day35/                              day80/  'thermo lecture 11'/
     day36/                              day81/  'thermo lecture 12'/
     day37/                              day82/  'thermo lecture 13'/
     day38/                              day83/  'thermo lecture 14'/
     day39/                              day84/  'thermo lecture 15'/
     day4/                               day85/  'thermo lecture 16'/
     day40/                              day86/  'thermo lecture 5'/
     day41/                              day87/  'thermo lecture 8'/
     day42/                              day88/  'thermo lecture 9'/
     day43/                              day89/   Two-tier-Application
     day44/                              day9/    var/


    HP@PRANAB MINGW64 /c/Pranab (main)
    $ vim createDirectories.sh

    #!/bin/bash
    
    prefix=$1
    start=$2
    end=$3
    
    for (( i=start; i<=end; i++ ))
    do
        mkdir "${prefix}${i}"
    done
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ chmod +x createDirectories.sh
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ./createDirectories.sh Movie 20 50
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ls
     2024_GIT_TUTORIAL/                  Movie26/             node-cicd
     90DaysOfDevOps/                     Movie27/             open_source
    '90DaysOfDevOps(LondheSubham153)'/   Movie28/            'Original Documents'/
     ansible_playbook                    Movie29/             Photo.jpg
     ansible_roles                       Movie30/             photos/
     ansible-inventory                   Movie31/             Pranab
    'bhai document.pdf'                  Movie32/             Prolog/
    'CIC-IOT(Attacks).pdf'               Movie33/             prometheus_grafana
     connecting-instances/               Movie34/            'Python(Jupiter)'/
     createDirectories.sh*               Movie35/             Python_Data-Types_Assignment.ipynb
     Cryptography1.zip                   Movie36/             README.md
    'DevOps & CloudComputing'/           Movie37/             Sample-Github-Actions-Workflow/
     docker_volume                       Movie38/             ShellScripts/
     Dockerfile-multi-stage              Movie39/             Software/
     Exam_Folder/                        Movie40/             Springboot_bankapp_Kubernetes
     Git/                                Movie41/             terraform_ec2
     HTML/                               Movie42/             terraform_EC2_Data_Variable_Output
    'IMPETUS GURUKUL (OLD COURSE)'/      Movie43/            'thermo lecture 10'/
     JAVA/                               Movie44/            'thermo lecture 11'/
     kuberentes_notes_app                Movie45/            'thermo lecture 12'/
     Lec-13.ppt                          Movie46/            'thermo lecture 13'/
     Lec-14.ppt                          Movie47/            'thermo lecture 14'/
     Lec-15.ppt                          Movie48/            'thermo lecture 15'/
    'math linear algebra'/               Movie49/            'thermo lecture 16'/
     metal/                              Movie50/            'thermo lecture 5'/
     Movie20/                            Movies/             'thermo lecture 8'/
     Movie21/                            MyFolder1/          'thermo lecture 9'/
     Movie22/                            MyFolder2/           Two-tier-Application
     Movie23/                            MyProject/           var/
     Movie24/                            newfolder/
     Movie25/                           'Nimcet Documents'/


*) Create a Script to Backup All Your Work:

  Backups are an important part of a DevOps Engineer's day-to-day activities. The video in the references will help you understand how a DevOps Engineer takes backups (it can feel a bit difficult but keep 
  trying, nothing is impossible).

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ vim backup.sh
    
    #!/bin/bash
    
    # Directory to back up (you can change this to your working directory)
    SOURCE_DIR="$HOME/my-work"
    
    # Backup destination directory
    BACKUP_DIR="$HOME/backups"
    
    # Create backup directory if it doesn't exist
    mkdir -p "$BACKUP_DIR"
    
    # Generate filename with current date and time
    TIMESTAMP=$(date +"%Y-%m-%d_%H-%M-%S")
    BACKUP_FILE="$BACKUP_DIR/work_backup_$TIMESTAMP.tar.gz"
    
    # Create the backup
    tar -czf "$BACKUP_FILE" "$SOURCE_DIR"
    
    echo "✅ Backup completed: $BACKUP_FILE"

    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ chmod +x backup.sh
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ./backup.sh
    tar: Removing leading `/' from member names
    tar: /c/Users/HP/my-work: Cannot stat: No such file or directory
    tar: Exiting with failure status due to previous errors
    ✅ Backup completed: /c/Users/HP/backups/work_backup_2025-05-14_22-06-05.tar.gz

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ cd /c/Users/HP/backups/
    HP@PRANAB MINGW64 ~/backups
    $ ls
    work_backup_2025-05-14_22-06-05.tar.gz


*) Read About Cron and Crontab to Automate the Backup Script:

    Cron is the system's main scheduler for running jobs or tasks unattended. A command called crontab allows the user to submit, edit, or delete entries to cron. A crontab file is a user file that holds the 
    scheduling information.

*) Read About User Management:
    
    A user is an entity in a Linux operating system that can manipulate files and perform several other operations. Each user is assigned an ID that is unique within the system. IDs 0 to 999 are assigned to          system users, and local user IDs start from 1000 onwards.
    Create 2 users and display their usernames.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ vim create_users.sh
    
    #!/bin/bash
    
    # Usernames to create
    USER1="useralpha"
    USER2="userbeta"
    
    # Create users
    sudo useradd "$USER1"
    sudo useradd "$USER2"
    
    # Show the usernames
    echo "✅ Created users:"
    echo "$USER1"
    echo "$USER2"
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ chmod +x create_users.sh
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ sudo ./create_users.sh
    
    ✅ Created users:
    useralpha
    userbeta
