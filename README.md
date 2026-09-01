<p align="center">
<img src="https://i.imgur.com/p7eKHoq.png" height="40%" width="60%" alt="Linux"/>
</p>
<h1>Linux Exercise: Navigation</h1>

In this exercise, I practiced fundamental Linux navigation commands by completing a series of terminal-based tasks. 

Credit to Colt Steele’s Udemy course, **The Linux Command Line Bootcamp: Beginner to Power User**, for providing both the exercise and the foundational knowledge needed to complete it.
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

To get started, I opened the terminal using the `Ctrl+Alt+T` keyboard shortcut. I used `pwd` (“print working directory”) to determine my current location and confirmed that I was in my home directory. I then used `ls` to view its contents. Since the `Farm` folder was located on my Desktop, I navigated into the `Desktop` directory with `cd`, listed its contents with `ls`, and then used `cd` again to enter the `Farm` directory. Finally, I used `pwd` to confirm my current location.

Although my shell prompt already displays `~/Desktop/Farm`, I intentionally used `pwd` so I could practice the command and build the habit of verifying my current working directory.

<br />
<br />

**2. List the contents of the `Farm` directory.**
<p>
<img src="https://i.imgur.com/n1Grcfc.png" height="100%" width="100%"/>
</p>

After confirming that I was in the `Farm` directory, I used `ls` to list its contents. The directory contained two subdirectories: `Coop` and `Stable`.

<br />
<br />

**3. "Move" into the `Coop` folder.**
<p>
<img src="https://i.imgur.com/8QsNXUc.png" height="100%" width="100%"/>
</p>

I used `cd Coop` to navigate into the `Coop` directory, then used `pwd` to verify my new working directory.

<br />
<br />

**4. List the contents of the `Coop` folder.**
<p>
<img src="https://i.imgur.com/B1B3KFa.png" height="100%" width="100%"/>
</p>

I used `ls` to list the contents of the `Coop` directory and found two subdirectories: `Chickens` and `Geese`.

<br />
<br />

**5. "Move" into the `Chickens` folder.**
<p>
<img src="https://i.imgur.com/BEpPC58.png" height="100%" width="100%"/>
</p>

I used `cd Chickens` to navigate into the `Chickens` directory, then verified my location with `pwd`.

<br />
<br />

**6. List out the chickens in the `Chickens` folder.  How many are there?**
<p>
<img src="https://i.imgur.com/Moayx5T.png" height="100%" width="100%"/>
</p>

Once inside the `Chickens` directory, I used `ls` to list its contents. There were six chickens: Buckbeak, Elvis, Ethel, Frida, Hippo, and Jaba.

<br />
<br />

**7. One of the chickens is younger than the others; which one is it? (Which file in the `Chickens` folder has the most recent modification time?) Use a command to figure it out!**
<p>
<img src="https://i.imgur.com/A8XqUYP.png" height="100%" width="100%"/>
</p>

To determine which chicken was the youngest (i.e., had the most recent modification time), I used `ls -l`, which displays a long listing containing details such as file permissions, ownership, size, and modification time. Comparing the modification times showed that `Buckbeak` was the most recently modified file: `Buckbeak` had a modification time of 9:07 PM, while the others showed 6:46 PM.

<br />
<br />

**8. In a ***single*** command, move from the `Chickens` directory to the `Geese` directory. Consult the folder structure written out above if needed.**
<p>
<img src="https://i.imgur.com/n9cgpJN.png" height="100%" width="100%"/>
</p>

I practiced both absolute and relative paths for this step. First, I used the absolute path `cd ~/Desktop/Farm/Coop/Geese`. I then returned to the `Chickens` directory and navigated back to `Geese` using the relative path `cd ../Geese`.

An absolute path identifies a location from a fixed starting point, while a relative path describes a location in relation to the current working directory. In `cd ../Geese`, `..` moves up one level from `Chickens` to `Coop`, and `Geese` then moves down into the neighboring directory.

<br />
<br />

**9. How many geese (files) are in the `Geese` directory?**
<p>
<img src="https://i.imgur.com/BliOXtf.png" height="100%" width="100%"/>
</p>

I used `ls` to list the contents of the `Geese` directory. There were four geese: Amelia, Boris, Lucy, and Muffin.

<br />
<br />

**10. One of the geese is sitting on a golden egg! It's larger than the other geese. Which one is it? (Which file in the `Geese` folder is the largest?) Use a command to figure it out!**
<p>
<img src="https://i.imgur.com/LFYJaNf.png" height="100%" width="100%"/>
</p>

I used `ls -l` to view detailed information about the files, including their sizes in bytes. Amelia, Boris, and Lucy were each 0 bytes, while Muffin was 15 bytes. Therefore, Muffin was the largest file (the goose sitting on the golden egg).

<br />
<br />

**11. Navigate to the `Horses` directory. Consult the folder structure written out above, if needed.**
<p>
<img src="https://i.imgur.com/scbZcmf.png" height="100%" width="100%"/>
</p>

Although I could have referred to the folder structure provided in the exercise, I wanted to determine the route myself. I used `ls` with directory paths to inspect the surrounding folder structure, then used a relative path with `cd` to navigate from `Geese` to `Horses`.

<br />
<br />

**12. How many horses are in the `Horses` directory?**
<p>
<img src="https://i.imgur.com/5FVjOdH.png" height="100%" width="100%"/>
</p>

I used `ls` to list the visible contents of the `Horses` directory and found four horses: Archer, Buttons, Cookie, and Jett.

<br />
<br />

**13. Wait! There is a hidden horse in the `Horses` directory! What is its name?**
<p>
<img src="https://i.imgur.com/muklrV9.png" height="100%" width="100%"/>
</p>

To reveal hidden files and directories, I used `ls -a`. Three additional entries appeared: `.`, `..`, and `.Troy`. The `.` entry represents the current directory, while `..` represents its parent directory. Because Linux filenames beginning with `.` are hidden by default, `.Troy` was the hidden horse (get it? Troy? hidden horse?).

<br />
<br />

**14. Bonus: List out the contents of the Horses directory as a comma-separated list. You'll need to dig into the man pages to find the correct option. Perhaps search the ls man page for "comma"?**
<p>
<img src="https://i.imgur.com/jlFiRWA.png" height="100%" width="100%"/>
</p>

For the bonus task, I needed to find an `ls` option that would display the directory contents as a comma-separated list. Rather than searching online, I used `man ls` to consult the command’s manual page.

<br />
<br />

<p>
<img src="https://i.imgur.com/MYXR1vM.png" height="100%" width="100%"/>
</p>

Within a man page, `/` can be used to search for text. I searched using `/comma` and pressed `n` to move through matching results until I found the `-m` option, which formats entries as a comma-separated list.

<br />
<br />

<p>
<img src="https://i.imgur.com/Bj79qN5.png" height="100%" width="100%"/>
</p>

I pressed `q` to exit the man page and returned to the terminal, where I ran `ls -m` to complete the bonus task.

<br />
<br />

<p>
✨ Building a strong foundation is important when learning any new technology. This exercise helped me become more comfortable navigating the Linux filesystem, working with relative and absolute paths, using command options, and consulting man pages when I need to find information on my own.
</p>
<br />
