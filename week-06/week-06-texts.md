---
layout: page
title: Texts
---

### Introduction

This week we're going to learn how to work with digitized historical texts. In Part I you will explore the process of digitizing text itself. 

In Part II you will learn how to get text and turn it into data. In Part III you apply some of the skills you learned in the Voyant tutorial to do some basic text analysis. To learn these skills, we will be looking at a common type of historical document: newspapers.

### Part I: Digital Text

To understand how digital text gets stored in databases, we'll be examining one of the largest free archives of U.S. newspapers: the Library of Congress's *Chronicling America* database. This database allows users to search for newspapers published across the United States over more than one hundred years. But how does this database work and what goes on under the hood?

Navigate to the Advanced Search tab at Chronicling America: <https://chroniclingamerica.loc.gov/>. Perform a search that returns newspapers that were printed on Halloween in the year 1900. 

- How many results are there?
- Where are *three states* that are represented in these results?

Change your Advanced Search to narrow it down further: newspapers that were printed `on Halloween` in the year `1900`, in the state of `Minnesota`, and that contain the word `halloween`. Copy and paste the resulting URL address from your results page into a plain text editor - typically TextEdit for Mac or Notepad for Windows. This type of URL acts as a set of instructions to the database that tells it what kind of results to show you based on certain "parameters" (such as the date or state of publication). 

Re-paste a *second* version of the same URL in your text editor and then try to **modify the text of the URL** so that if you load the URL in a web browser it returns newspapers that meet the following criteria:
  
- Printed on Christmas Day exactly one hundred years ago
- In the state of Arizona
- Containing the word `christmas`

**Hint**: your original URL might have some confusing symbols. If you're having trouble, here is a cleaned-up version of the original URL that is easier to read and then modify to fit the above parameters: `https://chroniclingamerica.loc.gov/search/pages/results/?state=Minnesota&dateFilterType=range&date1=10/31/1900&date2=10/31/1900&ortext=halloween`

Once you have successfully changed the URL and gotten search results that match the above criteria, choose one of the newspapers from these results (don't just choose the first one) and choose a story that mentions `christmas`. Zoom in and skim through the story. Now click on the `Text` link at the top of the viewer (next to `PDF`). Use your browser's find/search to try and relocate the story you just skimmed on this page. 

- Can you still understand it? Are any words difficult to understand? 

What you are seeing are the results of `Optical Character Recognition (OCR)` that we talked about earlier in the semester, in which a computer tries to "translate" a photographic *image* of text into *actual* text that you can analyze - what's known as "machine-readable" text.

Raise your hand and notify Cameron that you've reached this point. If other people are getting stuck, offer to help. If people are still working, try out a bonus exercise:

Come up with a URL that returns newspapers:

- Published on your birthday one hundred years ago
- Mentions the word "women" and "suffrage" within 10 words of each other

As a class:

- What were the results of your particular paper?
- What are some of the implications that this OCR process might have for digital text analysis like the kind you read about for today? 
- How does this relate to some of the readings and themes from earlier weeks?


### Part II: Processing Text

In this section, we're going to try and process and assemble text so that you can perform analysis on it. First, create a new folder on your computer named `week-06`. 

On the same page that shows the OCR'd version of your newspaper page (ex. <https://chroniclingamerica.loc.gov/lccn/sn84020558/1918-12-25/ed-1/seq-9/ocr/>, scroll down to the bottom of the page and click on the `txt` link. This is a link to a file that is *only* the raw, OCR'd text (and does not include any metadata. If you click on that link it will bring you to a URL that has ".txt" at the end. This means that your browser is showing you a text file rather than a webpage file (ex. if it ended in ".html").

Back in your browser, save the OCR text file into the `week-06` folder you created. Now you need to rename the file so that it tells you information about where it came from (its metadata). Instead of making up a name, go back to your browser and look at the URL. It should contain unique information that identifies which page, issue, and newspaper the text came from. 

- `sn84020558`: the unique ID of that newspaper title (ex. "The New York Times") 
- `1918-12-25`: the date of the issue
- `ed-1`: the edition
- `seq-9`: the page number (in this case, page 9). 

Rename the text file you just saved so that it includes this information, each separated by an underscore character ("_"). For the above example, this would look like `sn84020558_1918-12-25_ed-1_seq-9.txt` Although there's no perfect way to do this, at least now you've captured a fair amount of metadata about this file.

For the rest of Part II, download the Jupyter Notebook for [Week 6: Text]({{site.baseurl}}/week-06/week-06-text.ipynb) into your `week-06` folder, open it, and start to work through it.

### Part III: Analyzing Text

We're going to take a break from Python and try out Voyant Tools, which is an online interface for exploring patterns in text. 

- Download [this text file]({{site.baseurl}}/week-06/19191225_TheWashingtonHerald.txt), which is one that I stitched together from a 1919 Christmas Day edition of a single newspaper, the Washington Herald.
- Go to: <https://voyant-tools.org/>.
- Upload the text file to Voyant.

In groups of three, explore the Voyant interface. You can look at [Voyant Help](https://voyant-tools.org/docs/#!/guide/start) and try to figure out what the different tools are showing you.

As a class:

- Are there patterns that you notice in your text?
- Which of these tools seems most useful for historical research?
- How might the different tools be applied?
- What are their limitations?