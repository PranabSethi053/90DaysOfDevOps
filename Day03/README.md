*) View the content of a file and display line numbers.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ cat -n filename.txt
     1  The Indian Armed Forces on Wednesday (May 7, 2025) launched ‘Operation Sindoor’, hitting terrorist infrastructure in Pakistan and Pakistan-occupied Jammu and Kashmir, a government release read. India          exercised its right to act on terror, Foreign Secretary Vikram Misri said on the launch of military strikes on nine targets in Pakistan and Pakistan Occupied Jammu and Kashmir (POJK) under ‘Operation             Sindoor’ while stressing that the actions were “measured, non-escalatory, proportionate, and responsible” and focused on dismantling the terrorist infrastructure and disabling terrorists likely to be sent        across to India.
     2
     3
     4
     5
     6  Also read | Pakistan Army vows to respond to Indian air strikes.
     7
     8  The strikes on the nine targets, four in Pakistan and five in POJK, were conducted between 01:05Am to 01:30AM on Wednesday. No military establishments were targeted and there have been no reports of           collateral damage so far, she said. However, Pakistan has claimed several civilian causalities including women and children.
     9
    10  Operation Sindoor: Commercial flights suspended in northern parts of India.
    11
    12
    13  In a statement shortly after the Indian statement, DG ISPR said that all planes of Pakistan Air Force are airborne. “All strikes were made by India from its own airspace. Pakistan will respond to it at a     time and place of its own choosing. It will not go unanswered. The temporary pleasure of India will be replaced by enduring grief,” it stated.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ nl filename.txt
    1  The Indian Armed Forces on Wednesday (May 7, 2025) launched ‘Operation Sindoor’, hitting terrorist infrastructure in Pakistan and Pakistan-occupied Jammu and Kashmir, a government release read. India          exercised its right to act on terror, Foreign Secretary Vikram Misri said on the launch of military strikes on nine targets in Pakistan and Pakistan Occupied Jammu and Kashmir (POJK) under ‘Operation             Sindoor’ while stressing that the actions were “measured, non-escalatory, proportionate, and responsible” and focused on dismantling the terrorist infrastructure and disabling terrorists likely to be sent        across to India.




     2  Also read | Pakistan Army vows to respond to Indian air strikes.

     3  The strikes on the nine targets, four in Pakistan and five in POJK, were conducted between 01:05Am to 01:30AM on Wednesday. No military establishments were targeted and there have been no reports of           collateral damage so far, she said. However, Pakistan has claimed several civilian causalities including women and children.

     4  Operation Sindoor: Commercial flights suspended in northern parts of India.


     5  In a statement shortly after the Indian statement, DG ISPR said that all planes of Pakistan Air Force are airborne. “All strikes were made by India from its own airspace. Pakistan will respond to it at a      time and place of its own choosing. It will not go unanswered. The temporary pleasure of India will be replaced by enduring grief,” it stated.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ less -N filename.txt
    1 The Indian Armed Forces on Wednesday (May 7, 2025) launched ‘Operation Sindoor’, hitting terrorist infrastructure in Pakistan and Pakistan-occupied Jammu and Kashmir, a government release read. India ex        1 ercised its right to act on terror, Foreign Secretary Vikram Misri said on the launch of military strikes on nine targets in Pakistan and Pakistan Occupied Jammu and Kashmir (POJK) under ‘Operation Sind        1 oor’ while stressing that the actions were “measured, non-escalatory, proportionate, and responsible” and focused on dismantling the terrorist infrastructure and disabling terrorists likely to be sent a        1 cross to India.
    2
    3
    4
    5
    6 Also read | Pakistan Army vows to respond to Indian air strikes.
    7
    8 The strikes on the nine targets, four in Pakistan and five in POJK, were conducted between 01:05Am to 01:30AM on Wednesday. No military establishments were targeted and there have been no reports of col        8 lateral damage so far, she said. However, Pakistan has claimed several civilian causalities including women and children.
    9
    10 Operation Sindoor: Commercial flights suspended in northern parts of India.
    11
    12
    13 In a statement shortly after the Indian statement, DG ISPR said that all planes of Pakistan Air Force are airborne. “All strikes were made by India from its own airspace. Pakistan will respond to it at        13 a time and place of its own choosing. It will not go unanswered. The temporary pleasure of India will be replaced by enduring grief,” it stated.



    HP@PRANAB MINGW64 /c/Pranab (main)
    $ awk '{print NR, $0}' filename.txt
    1 The Indian Armed Forces on Wednesday (May 7, 2025) launched ‘Operation Sindoor’, hitting terrorist infrastructure in Pakistan and Pakistan-occupied Jammu and Kashmir, a government release read. India           exercised its right to act on terror, Foreign Secretary Vikram Misri said on the launch of military strikes on nine targets in Pakistan and Pakistan Occupied Jammu and Kashmir (POJK) under ‘Operation             Sindoor’ while stressing that the actions were “measured, non-escalatory, proportionate, and responsible” and focused on dismantling the terrorist infrastructure and disabling terrorists likely to be sent        across to 
    India.
    2
    3
    4
    5
    6 Also read | Pakistan Army vows to respond to Indian air strikes.
    7
    8 The strikes on the nine targets, four in Pakistan and five in POJK, were conducted between 01:05Am to 01:30AM on Wednesday. No military establishments were targeted and there have been no reports of            collateral damage so far, she said. However, Pakistan has claimed several civilian causalities including women and children.
    9
    10 Operation Sindoor: Commercial flights suspended in northern parts of India.
    11
    12
    13 In a statement shortly after the Indian statement, DG ISPR said that all planes of Pakistan Air Force are airborne. “All strikes were made by India from its own airspace. Pakistan will respond to it at a      time and place of its own choosing. It will not go unanswered. The temporary pleasure of India will be replaced by enduring grief,” it stated.
    

*) Change the access permissions of files to make them readable, writable, and executable by the owner only.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ls -ltr
    -rw-r--r-- 1 HP 197121     1458 May  8 17:46  filename.txt
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ chmod 700 filename.txt
    -rwx------ 1 HP 197121     1458 May  8 17:46  filename.txt

*) Check the last 10 commands you have run.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ history | tail -n 10
    537  ls
    538  ls -ltr
    539  mount | grep /mnt
    540  mount | grep /mnt
    541  ls -ltr
    542  chmod 700 filename.txt
    543  ls -ltr
    544  history
    545  cd /c/Pranab/
    546  history | tail -n 10

*) Remove a directory and all its contents.

    HP@PRANAB MINGW64 /c/Pranab/myfolder (main)
    $ vim file.txt
    HP@PRANAB MINGW64 /c/Pranab/myfolder (main)
    $ cat file.txt
    The Indian Armed Forces on Wednesday (May 7, 2025) launched ‘Operation Sindoor’, hitting terrorist infrastructure in Pakistan and Pakistan-occupied Jammu and Kashmir, a government release read. India             exercised its right to act on terror, Foreign Secretary Vikram Misri said on the launch of military strikes on nine targets in Pakistan and Pakistan Occupied Jammu and Kashmir (POJK) under ‘Operation             Sindoor’ while stressing that the actions were “measured, non-escalatory, proportionate, and responsible” and focused on dismantling the terrorist infrastructure and disabling terrorists likely to be sent        across to India.
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ rm -rf myfolder/
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ ls myfolder
    ls: cannot access 'myfolder': No such file or directory

*) Create a fruits.txt file, add content (one fruit per line), and display the content.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ cat > fruits.txt
    Apple
    Banana
    Mango
    Orange
    Grapes
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ cat fruits.txt
    Apple
    Banana
    Mango
    Orange
    Grapes


*) Add content in devops.txt (one in each line) - Apple, Mango, Banana, Cherry, Kiwi, Orange, Guava. Then, append "Pineapple" to the end of the file.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ echo -e "Apple\nMango\nBanana\nCherry\nKiwi\nOrange\nGuava" > devops.txt
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ cat devops.txt
    Apple
    Mango
    Banana
    Cherry
    Kiwi
    Orange
    Guava
    
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ echo "Pineapple" >> devops.txt
    HP@PRANAB MINGW64 /c/Pranab (main)
    
    $ cat devops.txt
    Apple
    Mango
    Banana
    Cherry
    Kiwi
    Orange
    Guava
    Pineapple

*) Show the first three fruits from the file in reverse order.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ head -n 3 devops.txt | tac | rev
    ananaB
    ognaM
    elppA


*) Show the bottom three fruits from the file, and then sort them alphabetically.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ tail -n 3 devops.txt | sort
    Guava
    Orange
    Pineapple

*) Create another file Colors.txt, add content (one color per line), and display the content.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ echo -e "Red\nBlue\nGreen\nYellow\nOrange\nPurple\nWhite" > Colors.txt
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ cat Colors.txt
    Red
    Blue
    Green
    Yellow
    Orange
    Purple
    White

*) Add content in Colors.txt (one in each line) - Red, Pink, White, Black, Blue, Orange, Purple, Grey. Then, prepend "Yellow" to the beginning of the file.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ echo -e "Red\nPink\nWhite\nBlack\nBlue\nOrange\nPurple\nGrey" > Colors.txt
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ echo "Yellow" | cat - Colors.txt > temp && mv temp Colors.txt
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ cat Colors.txt
    Yellow
    Red
    Pink
    White
    Black
    Blue
    Orange
    Purple
    Grey

*) Find and display the lines that are common between fruits.txt and Colors.txt.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ comm -12 <(sort fruits.txt) <(sort Colors.txt)
    Orange
    HP@PRANAB MINGW64 /c/Pranab (main)
    $ grep -Fxf fruits.txt Colors.txt
    Orange


*) Count the number of lines, words, and characters in both fruits.txt and Colors.txt.

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ wc fruits.txt Colors.txt
     5  5 33 fruits.txt
     9  9 52 Colors.txt
    14 14 85 total

    HP@PRANAB MINGW64 /c/Pranab (main)
    $ wc -l -w -c fruits.txt Colors.txt
     5  5 33 fruits.txt
     9  9 52 Colors.txt
    14 14 85 total
