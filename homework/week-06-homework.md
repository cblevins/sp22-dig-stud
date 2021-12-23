---
layout: page
title: Week 6 Homework
---

In this homework you're going to reinforce more of the Python skills you learned in class in Week 4: use Python to open and read a bunch of text files, process them in some way, and then do some basic analysis. Refer back to the [in-class portion of Week 4]({{site.baseurl}}/week-04/week-04-data-wrangling.ipynb) to help you. Once again, please alternate Markdown cells with Code cells where you explain each step. 

### The Data

For this week we're going to use diary entries from the diary of Martha Ballard, a midwife from Maine made famous by Laurel Ulrich's *A Midwife's Tale*. A project at George Mason University digitized her diary and put it online. I've done some work on the entries, and am supplying you with two years' worth of Ballard's entries (1804 and 1805). Each of her entries for these two years are contained in a separate text file that I've already preprocessed, cleaned up, and put into all lowercase.

### Set Up
1. Create a new folder inside the `homework` folder on your computer called `week-06-homework`. Launch Anaconda Navigator and then create a new Jupyter Notebook inside this folder using the filename convention: `yourlastname-week-06-homework.ipynb`. 
2. [Download Martha Ballard's diary entries for 1804 and 1805]({{site.baseurl}}/homework/week-06-homework-data.zip) and put the file in your `week-06-homework` folder. Unzip this and rename the folder `data`. This is your directory of text files.
3. In your Jupyter Notebook: 
    - Import the `os` and `string` libraries
    - Use `os` to tell Python where to look for the data (text files)

### Wrangle the Data

The goal of this section is to take your hundreds of text files worth of diary entries and add them into two lists, one containing all of the diary entries for 1804 and one for 1805. You're going to do this through the following steps:

1. Make two new variables, `year_1804` and `year_1805`, and make them empty lists. This is where you're going to be adding individual entries for that year as items in your list.
2. Use `os.listdir()` to get a list of filenames contained in your data folder and assign it as a new variable
3. Write a `for` loop to go through your list of filenames and `open()` each diary entry read() its contents.
4. **Inside** that same `for` loop, then use an `if` statement to figure out which year the diary entry was written. Based on that, `append()` the entry to either your `year_1804` or `year_1805` list. 
    - Hint: this is going to require a new function, but one that is related to the `if f.endswith('.txt'):` in your Week 4 exercise. Try Googling to see if you can figure out what function to use.

### Analyze the Data

Let's do some basic analysis of Martha Ballard's diary entries for these two years. 

1. In which year did she write more entries?
2. What is Ballard's longest entry that she wrote in 1804 or 1805?
3. What is the shortest entry that she wrote?
4. What is the average length of her entries in 1804 vs. 1805?
    - Note: this is a tricky one that requires some thinking outside of the box or importing a library you haven't used yet - if you can't figure it out, feel free to skip it
5. What was the weather in Maine exactly 215 years ago from *today*? The goal is to generate a print statement that just prints out the sentence from that particular entry containing the weather.
    - Use a `for` loop to go back through your data files
    - Use an `if` statement to locate the correct text file based on its filename
    - `open()`, `read()`, and assign the contents of just that file to a new variable 
    - Use the `split()` function to create a new list, with each individual item being a different sentence from her diary entry. Think about what character you want to "split" on.
    - `print()` just the sentence that talks about the weather. To do this, you're going to tell Python which item inside your list of sentences you want to print using the brackets `[]` notation. **Annoying Python feature**: Python starts "counting" at 0 instead of 1. So to access the second item in your list, you'd use `print(somelist[3])` NOT `print(somelist[2])`. Fun right? :)
