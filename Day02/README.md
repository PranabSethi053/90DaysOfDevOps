*) Listing commands

        ls :- list the sub directories and files avaiable in the present directory
        HP@PRANAB MINGW64 /c/Pranab/A (main)
        $ ls
        MyDirectory/

        ls -a:- list all including hidden files and directory
        HP@PRANAB MINGW64 /c/Pranab/A (main)
        $ ls -a
        ./  ../  MyDirectory/

        ls *.exe:-list all the files having .exe extension.
        HP@PRANAB MINGW64 ~/Downloads
        $ ls *.exe
        Anaconda3-2024.06-1-Windows-x86_64.exe*   mingw-get-setup.exe*       tsetup-x64.5.4.0.exe*
        'Docker Desktop Installer.exe'*            Oracle_10g_XE.exe*        'vs_BuildTools (1).exe'*
 
        ls -i:- list the files and directories with index numbers inodes
        HP@PRANAB MINGW64 /c/Pranab (main)
        $ ls -i
        17732923532897668  2024_GIT_TUTORIAL/
        5348024557604388  90DaysOfDevOps/
        24488322973833778 '90DaysOfDevOps(LondheSubham153)'/
        21955048183442677  ansible_playbook
        14918173765700168  ansible_roles
        44473046320331890  ansible-inventory

        ls -d */:- list only directories.(we can also specify a pattern)
        HP@PRANAB MINGW64 /c/Pranab (main)
        $ ls -d */
        2024_GIT_TUTORIAL//                 'math linear algebra/'/             Software//
        '90DaysOfDevOps(LondheSubham153)/'/   metal//                           'thermo lecture 10/'/
        90DaysOfDevOps//                     Movies//                          'thermo lecture 11/'/


        
*)  Directory commands

        pwd :- print work directory. Gives the present working directory.
        HP@PRANAB MINGW64 /c/Pranab (main)
        $ pwd
        /c/Pranab

        cd path_to_directory :- change directory to the provided path
        HP@PRANAB MINGW64 ~
        $ cd /c/Pranab/
        HP@PRANAB MINGW64 /c/Pranab (main)

        cd ~  or just cd  :- change directory to the home directory
        HP@PRANAB MINGW64 /c/Pranab (main)
        $ cd
        HP@PRANAB MINGW64 ~
        $ cd /c/Pranab
        HP@PRANAB MINGW64 /c/Pranab (main)
        $ cd ~
        HP@PRANAB MINGW64 ~
        $

        cd - :- Go to the last working directory.
        HP@PRANAB MINGW64 /c/Pranab/90DaysOfDevOps (master)
        $ cd -
        /c/Users/HP
        HP@PRANAB MINGW64 ~

        cd .. :- change directory to one step back.
        HP@PRANAB MINGW64 /c/Pranab/90DaysOfDevOps (master)
        $ cd ..
        HP@PRANAB MINGW64 /c/Pranab (main)

        cd ../.. :- Change directory to 2 levels back.
        HP@PRANAB MINGW64 /c/Pranab/90DaysOfDevOps (master)
        $ cd ../..
        HP@PRANAB MINGW64 /c

        *) mkdir  directoryName :- to make a directory in a specific location.
                HP@PRANAB MINGW64 /c/Pranab (main)
                $ mkdir newfolder
                HP@PRANAB MINGW64 /c/Pranab (main)
                $ ls
                MyFolder1/                         'thermo lecture 8'/
                MyFolder2/                         'thermo lecture 9'/
                newfolder/                          var/

        *) mkdir .NewFolder    # make a hidden directory (also . before a file to make it hidden)
        
                HP@PRANAB MINGW64 /c/Pranab (main)
                $ mkdir .NewFolder
                HP@PRANAB MINGW64 /c/Pranab (main)
                $ ls -a
                ./                                  JAVA/                  'Python(Jupiter)'/
                ../                                 kuberentes_notes_app    Python_Data-Types_Assignment.ipynb
                .git/                               Lec-13.ppt              README.md
                .NewFolder/

        *) mkdir A B C D                  #make multiple directories at the same time
        
                HP@PRANAB MINGW64 /c/Pranab (main)
                $ mkdir A B C D
                HP@PRANAB MINGW64 /c/Pranab (main)
                $ ls
                A                                  Lec-14.ppt             Sample-Github-Actions-Workflow
                ansible-inventory                  metal                  Springboot_bankapp_Kubernetes
                B                                  Movies                 terraform_ec2
                'bhai document.pdf'                 MyFolder1              terraform_EC2_Data_Variable_Output
                C                                  MyFolder2             'thermo lecture 10'
                D

        *) mkdir /home/user/Mydirectory   # make a new folder in a specific location
                
                HP@PRANAB MINGW64 / (main)
                $ mkdir home/user/MyDirectory
                HP@PRANAB MINGW64 / (main)
                $ cd home/user/MyDirectory/
                HP@PRANAB MINGW64 /home/user/MyDirectory (main)
                $ ls      

       *)  mkdir -p  A/B/C/D              # make a nested directory
       
                HP@PRANAB MINGW64 /c/Pranab (main)
                $ mkdir -p  A/B/C/D
                HP@PRANAB MINGW64 /c/Pranab (main)
                $ ls
                 2024_GIT_TUTORIAL/                 'Nimcet Documents'/
                 90DaysOfDevOps/                     node-cicd
                '90DaysOfDevOps(LondheSubham153)'/   open_source
                 A/                                 'Original Documents'/
                HP@PRANAB MINGW64 /c/Pranab (main)
                $ cd A
                HP@PRANAB MINGW64 /c/Pranab/A (main)
                $ ls
                B/
                HP@PRANAB MINGW64 /c/Pranab/A (main)
                $ cd B
                HP@PRANAB MINGW64 /c/Pranab/A/B (main)
                $ ls
                C/
                HP@PRANAB MINGW64 /c/Pranab/A/B (main)
                $ cd C
                HP@PRANAB MINGW64 /c/Pranab/A/B/C (main)
                $ ls
                D/
                HP@PRANAB MINGW64 /c/Pranab/A/B/C (main)
                $ cd D
                HP@PRANAB MINGW64 /c/Pranab/A/B/C/D (main)
                $ ls   
                
