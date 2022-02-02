---
layout: page
title: File Manager in Reclaim Hosting
---

The goal of this activity is to get more comfortable with using the File Mangager in Reclaim Hosting (accessed through the cPanel). If you had trouble creating a sandbox directory, please review [Creating a "Sandbox" on Reclaim Hosting]({{site.baseurl}}/in-class/reclaim-hosting-sandbox) and make sure you have a folder called `sandbox` inside your `public_html` folder in File Manager.

Although you are going to be using your Reclaim Hosting server space to host a personal website, you can also host individual files. To demonstrate, we're going to work with an image of Professor Blevins's ferocious cat.

### Uploading an image to File Manager
- Download the photo of Professor Blevins's cat from the `#in-class` Slack channel and save or move it into the `sp22-dig-stud` folder on your computer (leave the name as `prof-blevins-cat.jpeg`). 
- Log into reclaim hosting, go to cPanel -> File Manager and then navigate to your `sandbox` folder
- Add the photo you just downloaded from Slack into your `sandbox` folder using the Upload button at the top of File Manager.
- Go to `https://yourdomainname/sandbox/prof-blevins-cat.jpeg` and see if the photo shows up.

### Embedding an image in an HTML file
- Make sure you are inside the `sandbox` folder in File Manager
- Create a new HTML file by clicking +File and naming 
it `cat.html`
- Open the new file using the HTML Editor button (ignore the warnings)
- Inside the HTML Editor, write "This is Professor Blevins's beautiful cat:"
- Click the `<>Source` button, and then copy and paste this line of code directly *before* the line in your file that says `</body>`: `<p><img alt="" src="https://cameronblevins.org/teaching/sp22-dig-stud/sandbox/prof-blevins-cat.jpeg" style="height: 267px; width: 200px;" /></p>`
- Go to `https://yourdomainname/sandbox/cat.html` and see if the page is showing an embedded photo. 