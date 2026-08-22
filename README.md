<p align="center">
<img src="https://i.imgur.com/p7eKHoq.png" height="40%" width="60%" alt="Linux"/>
</p>
<h1>Linux Navigation Exercise</h1>

In this exercise, I used fundamental navigation commands in a Linux terminal to complete various tasks. 

Credit to Colt Steele's Udemy course **The Linux Command Line Bootcamp: Beginner To Power User** for both the exercise and teaching me the knowledge to complete it!
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
  - n
  - q

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

Using the `ls -l` command like earlier, I could view more details about the files in the directory. The column to the left of the one showing the month (Aug) shows the size of the file in bytes. The Amelia, Boris, and Lucy files have a size of 0 bytes (they are empty), and the Muffin file has a size of 15 bytes; this means the Muffin is sitting on the golden egg/is the largest file.

<br />
<br />

**11. Navigate to the `Horses` directory. Consult the folder structure written out above, if needed.**
<p>
<img src="https://i.imgur.com/scbZcmf.png" height="100%" width="100%"/>
</p>

While I could have referred to the folder structure above, I wanted to try navigating to the `Horses` directory without doing so. I used the `ls` command with absolute paths to get a layout of the folders in each directory and map out a path, then used the `cd` command with a relative path to navigate from the `Geese` directory to the `Horses` directory.

<br />
<br />

**12. How many horses are in the `Horses` directory?**
<p>
<img src="https://i.imgur.com/5FVjOdH.png" height="100%" width="100%"/>
</p>

Using the `ls` command, I determined that there were 4 horses present: Archer, Buttons, Cookie, and Jett.

<br />
<br />

**13. Wait! There is a hidden horse in the `Horses` directory! What is its name?**
<p>
<img src="https://i.imgur.com/muklrV9.png" height="100%" width="100%"/>
</p>

To find the name of the hidden horse, I used the `ls -a` command; the `-a` option ensures that hidden files and directories will also be listed. Three new results appeared: `.`, `..`, and `.Troy`. `.` refers to the current directory, `..` refers to one directory above the current directory, and `.Troy` is the hidden horse (get it? Troy? hidden horse?).

<br />
<br />

**14. Bonus: List out the contents of the Horses directory as a comma-separated list. You'll need to dig into the man pages to find the correct option. Perhaps search the ls man page for "comma"?**
<p>
<img src="https://i.imgur.com/jlFiRWA.png" height="100%" width="100%"/>
</p>

I used the `man` command (short for manual) to see what options I could use with the `ls` command to create a comma-separated list. Here's what I first saw when I entered the `man ls` command.

<br />
<br />

<p>
<img src="https://i.imgur.com/MYXR1vM.png" height="100%" width="100%"/>
</p>

Like the "Ctrl+F" keyboard shortcut, `/` can search for a specific string in a man page. Using `/comma` to search for every occurrence of the word "comma" and the `n` key to jump to each occurrence, I found that the `-m` option will separate the contents of a directory with commas.

<br />
<br />

<p>
<img src="https://i.imgur.com/Bj79qN5.png" height="100%" width="100%"/>
</p>

I returned to the terminal using the `q` key, then used the command `ls -m` to complete the bonus task.

<br />
<br />

<p>
✨ It is so important to learn and become comfortable with the fundamentals of any technology that you are new to, and this exercise definitely helped me get used to navigating and using the man pages.
</p>
<br />
