---
layout: page
title: Week 5 Homework
---

You're going to submit your second homework of the semester using a Jupyter Notebook. In this homework you're going to reinforce some of the skills you learned in class: use Python to open a text file, read its contents, turn its text into a `list`, and use a `for` loop to do some basic analysis. Refer back to the [in-class portion of Week 4]({{site.baseurl}}/week-04/week-04-data-wrangling.ipynb) to help you. Once again, please alternate Markdown cells with Code cells where you explain each step. 

### Get the Data

1. Create a new folder inside the `homework` folder on your computer called `week-05-homework`. Launch Anaconda Navigator and then create a new Jupyter Notebook inside this folder using the filename convention: `yourlastname-week-05-homework.ipynb`. 
2. Make a `data` folder inside your `week-05-homework` folder. This is where you're going to put the text files.
3. You're going to analyze two files. Rather than provide them for you, I want you to get some experience locating and downloading them "in the wild." For today we're going to use the Internet Archive, which is a large repository of material - including texts. I've chosen two history books printed by Northeastern University Press and that were uploaded to the Internet Archive by Northeastern University Library. Your first step is to locate them on the Internet Archive:
    - Jacqueline Barbara Carr, *After the Siege: A Social History of Boston, 1775-1800*
    - Amalie M. Kass, *Midwifery and Medicine in Boston: Walter Channing, M.D., 1786-1876*
4. The goal is to download two text files (ending in `.txt`) of these two books and put them inside your `data` folder. Use this page to try and figure out how to download the raw `.txt` file: <https://help.archive.org/hc/en-us/articles/360017781111-How-to-download-files>
5. You should know have a `week-05-homework` folder consisting of:
     - Your Jupyter Notebook
     - A folder called `data`
     - Two `.txt` files inside your `data` folder of the two above books

### Wrangle the Data

You're now going to load each file into your Jupyter Notebook. I would recommend just working with one file for now until you manage to get it all working. 

**Before you begin**, note that you're going to be working with much larger files and data than you did in class. Keep this in mind if you use a print statement to, say, print out the entire contents of a file - this could bog down your machine. I would recommend a workaround. For strings and lists, you can specify just particular parts of them using brackets [ ] immediately after the name of the variable and then numbers inside the variable separated by a colon. So if your variable is a list, then `print(somelistvariable[0:10])` will only print the first ten items of the list. If your variable is a string (ie. text), then `print(somestringvariable[0:10])` will only print the first ten characters of your string.

1. Import the necessary Python libraries `os` and `string`
2. Use `os` functions to tell Python where to look for the data (text files)
3. `open()` and then `read()` the text file, assigning a variable to its contents
4. Create a `list` consisting of words contained in the text contents using the `split()` function and assign it to a new variable. 
    - Note: this function takes any kind of text and breaks it up using whatever character you told it. In our in-class exercise, we used the hidden newline `\n` character in order to tell it to break up the string whenever it got to the end of a *line*. For this homework, I'd like you to create a list of *words* instead of *lines*. What equivalent "character" would you use instead of `\n`? If you're having trouble figuring this out, Google might have some help. :)
5. Now repeat the above steps for the second text (note: you'll want to name your variables to distinguish between the two - something like `text1` vs. `text2`, or `kass` vs. `carr`.

### Analyze the Data

Refer back to our in-person exercise to try and figure out answers to the following questions. I've included the names of relevant functions for each of them.

1. Which of the two books is longer in terms of their total number of words? `len()`
2. Which book has the longest *individual* word? `max()`, `len()`
3. How many *unique* words are used by each author? ie. Which author has a larger vocabulary? `lists`, `for loop`, `if...not in`, `append` 
    - Note: looping through a large text might take your computer awhile. If there is an asterisk on the left side of a cell - ie. [\*] - that means the cell is still working. Don't use a print statement here or it will take even longer. If you think it's frozen, try restarting the kernel.


Once you've completed the homework: **create a zip file ([Windows instructions](https://support.microsoft.com/en-us/help/14200/windows-compress-uncompress-zip-files), [Mac instructions](https://support.apple.com/guide/mac-help/compress-uncompress-files-folders-mac-mchlp2528/mac)) of your `week-05-homework` folder** and then upload it to: <https://www.dropbox.com/request/6DlmzXwe51JsbvFrlQ4c>.

 
