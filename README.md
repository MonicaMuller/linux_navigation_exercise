<p align="center">
<img src="https://i.imgur.com/p7eKHoq.png" height="40%" width="60%" alt="Linux"/>
</p>
<h1>Linux Navigation Exercise</h1>
Lorem ipsum
<br />

<h2>The Commands</h2>

- pwd
- ls
  - -l
  - -a
- cd
  - ..
- man
  - /

<h2>The Exercise</h2>

 The Farm folder contains the following subdirectories:

- Farm/
  - Coop/
    - Chickens/
    - Geese/
  - Stable/
    - Horses/

**ONLY use the terminal to accomplish the following:**

1. Open a new terminal window. Navigate to the `Farm` folder.
2. List the contents of the `Farm` directory.
3. "Move" into the `Coop` folder.
4. List the contents of the `Coop` folder.
5. "Move" into the `Chickens` folder.
6. List out the chickens in the `Chickens` folder. How many are there?
7. One of the chickens is younger than the others; which one is it? (Which file in the `Chickens` folder has the most recent modification time?) Use a command to figure it out!
8. In a **single** command, move from the `Chickens` directory to the `Geese` directory. Consult the folder structure written out above if needed.
9. How many geese (files) are in the `Geese` directory?
10. One of the geese is sitting on a golden egg! It's larger than the other geese. Which one is it? (Which file in the `Geese` folder is the largest?) Use a command to figure it out!
11. Navigate to the `Horses` directory. Consult the folder structure written out above, if needed.
12. How many horses are in the `Horses` directory?
13. Wait! There is a hidden horse in the `Horses` directory! What is its name?
14. Bonus: List out the contents of the Horses directory as a comma-separated list. You'll need to dig into the man pages to find the correct option. Perhaps search the ls man page for "comma"?

<h2>What I Did</h2>

**1. Open a new terminal window. Navigate to the `Farm` folder.**
<p>
<img src="https://i.imgur.com/r6iMPpB.png" height="100%" width="100%"/>
</p>

To get started, I opened the terminal using the `Ctrl+Alt+T` keyboard shortcut. To determine what directory I was currently in, I used the `pwd` command, which stands for "print working directory"; I found that I was in my home folder. I then used the `ls` command to see the files and folders in my home folder. Knowing that the `Farm` folder was on my Desktop, I used the `cd` command to navigate into my Desktop folder, the `ls` command to see what was in the folder, the `cd` command to go into the `Farm` folder, and lastly, the `pwd` command to confirm that I was in the `Farm` folder. (I am aware that my current working directory of `~/Desktop/Farm` does the same as the `pwd` command, but I want to get into the habit of using it and typing in the terminal)

<br />
<br />

**2. List the contents of the `Farm` directory.**
<p>
<img src="https://i.imgur.com/n1Grcfc.png" height="100%" width="100%"/>
</p>

In the previous step, I confirmed that I was in the `Farm` directory by using the `pwd` command. To list the contents of the directory I was currently in, I used the `ls` command and confirmed that the `Farm` directory contained two folders: `Coop` and `Stable`.

<br />
<br />

**3. "Move" into the `Coop` folder.**
<p>
<img src="https://i.imgur.com/8QsNXUc.png" height="100%" width="100%"/>
</p>

To move into the `Coop` folder, I used the `cd` command, then confirmed that I was in the folder using the `pwd` command.

<br />
<br />

**4. List the contents of the `Coop` folder.**
<p>
<img src="https://i.imgur.com/B1B3KFa.png" height="100%" width="100%"/>
</p>

I listed the contents of the `Coop` folder using the `ls` command and determined that the `Coop` folder contained two folders: `Chickens` and `Geese`.

<br />
<br />

**5. "Move" into the `Chickens` folder.**
<p>
<img src="https://i.imgur.com/BEpPC58.png" height="100%" width="100%"/>
</p>

I moved into the `Chickens` folder using the `cd` command, then used the `pwd` command to verify that I was in the `Chickens` folder.

<br />
<br />

**6. List out the chickens in the `Chickens` folder.  How many are there?**
<p>
<img src="https://i.imgur.com/Moayx5T.png" height="100%" width="100%"/>
</p>

Once I was in the chicken folder, I used the `ls` command to list out the chickens in the `Chickens` folder. I counted that there were 6 chickens present: Buckbeak, Elvis, Ethel, Frida, Hippo, and Jaba.

<br />
<br />

**7. One of the chickens is younger than the others; which one is it? (Which file in the `Chickens` folder has the most recent modification time?) Use a command to figure it out!**
<p>
<img src="https://i.imgur.com/A8XqUYP.png" height="100%" width="100%"/>
</p>

To determine which of the chickens was younger than the others, I used the `ls -l` command, since using the `-l` option displays more detail when listing the contents of a directory. In the second-to-last column, I saw that Buckbeak was younger than the others; Buckbeak had a modification time of 9:07 PM, and the other chickens had a modification time of 6:46 PM.

<br />
<br />

**8. In a ***single*** command, move from the `Chickens` directory to the `Geese` directory. Consult the folder structure written out above if needed.**
<p>
<img src="https://i.imgur.com/n9cgpJN.png" height="100%" width="100%"/>
</p>

I decided to navigate into the `Geese` directory using two different ways: an <ins>absolute path</ins> and a <ins>relative path</ins>. To summarize, a relative path is a path that only works relative to your current directory, while an absolute path works regardless of what your current directory is. I started with an absolute path by using the command `cd ~/Desktop/Farm/Coop/Geese`, then navigated back to the `Chickens` folder and then back again to the `Geese` folder using relative paths; the `cd ../Geese` command took me up one folder to the `Coop` directory and then down into the `Geese` folder.

<br />
<br />

**9. How many geese (files) are in the `Geese` directory?**
<p>
<img src="https://i.imgur.com/BliOXtf.png" height="100%" width="100%"/>
</p>

Similar to Step 6, I used the `ls` command and counted 4 geese in the `Geese` directory: Amelia, Boris, Lucy, and Muffin.

<br />
<br />

**10. One of the geese is sitting on a golden egg! It's larger than the other geese. Which one is it? (Which file in the `Geese` folder is the largest?) Use a command to figure it out!**
<p>
<img src="https://i.imgur.com/LFYJaNf.png" height="100%" width="100%"/>
</p>

Lorem ipsum

<br />
<br />

**11. Navigate to the `Horses` directory. Consult the folder structure written out above, if needed.**
<p>
<img src="https://i.imgur.com/scbZcmf.png" height="100%" width="100%"/>
</p>

Lorem ipsum

<br />
<br />

**12. How many horses are in the `Horses` directory?**
<p>
<img src="https://i.imgur.com/5FVjOdH.png" height="100%" width="100%"/>
</p>

Lorem ipsum

<br />
<br />

**13. Wait! There is a hidden horse in the `Horses` directory! What is its name?**
<p>
<img src="https://i.imgur.com/muklrV9.png" height="100%" width="100%"/>
</p>

Lorem ipsum

<br />
<br />

**14. Bonus: List out the contents of the Horses directory as a comma-separated list. You'll need to dig into the man pages to find the correct option. Perhaps search the ls man page for "comma"?**
<p>
<img src="https://i.imgur.com/jlFiRWA.png" height="100%" width="100%"/>
</p>

Lorem ipsum

<br />
<br />

<p>
<img src="https://i.imgur.com/MYXR1vM.png" height="100%" width="100%"/>
</p>

Lorem ipsum

<br />
<br />

<p>
<img src="https://i.imgur.com/Bj79qN5.png" height="100%" width="100%"/>
</p>

Lorem ipsum

<br />
<br />

<p>
✨ Lorem ipsum
</p>
<br />
