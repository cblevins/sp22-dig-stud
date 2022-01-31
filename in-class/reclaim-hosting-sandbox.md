---
layout: page
title: Creating a "Sandbox" on Reclaim Hosting
---

## Explore File Manager and `public_html`

Log into your Reclaim Hosting account click on cPanel. This is the overview page where you can manage a bunch of different aspects of your server account with Reclaim Hosting (such as URL domain names, setting up an email account based on your domain, etc.). Find `File Manager`and open this in a new browser tab, which will bring you to an interface showing you some folders. Much like your physical computer, your server space at Reclaim Hosting is organized into a collection of folders containing files, scripts, folders, etc. Don't worry about what all of them mean. For now, navigate to `public_html`. This is where you can add files, webpages, etc. that you want to be accessible by other people through an internet browser.

## Make a Sandbox Directory

Your first step is to make a "sandbox" folder in your `public_html` directory that is going to be your space to install and learn new tools. This is where you can mess around and try things out without worrying about anything breaking. The `sandbox` folder is going to be set up so that it can be accessed in the following way: `https://yourdomainnameurl/sandbox/`. When you start adding sub-folders or material within your `sandbox` folder they will be just be appended to that URL (ex. `https://yourdomainnameurl/sandbox/photo-of-my-adorable-cat.jpg`).

To create your sandbox:
- Make sure you are in File Manager (cPanel -> File Manager)
- Navigate to the `public_html` folder and make sure you are inside the folder
- Add a new folder within your `public_html` folder called `sandbox` (make sure it says `public_html` under "New folder will be created in:")
- Navigate to the folder. It should be empty. :)

## Add a file to your sandbox

Now let's try adding a file into your `sandbox` folder. While still in File Manager, click `+File` in the upper left, then name it `hello.html`. The `.html` ending tells File Manager what kind of file it is (in this case, an HTML webpage). Make sure it is created *inside* your sandbox folder, then click Create New File. You should see a new file inside your directory. Select it by clicking once, then click on HTML Editor towards the top of File Manager. Click the Edit button that appears in a pop-up, and you should be seeing a blank screen with some buttons at the top. Try writing a short message in the document, then click the Save button. 

In a new browser tab, navigate to: `https://yourdomainnameurl/sandbox/hello.html` and you should see your message. Congratulations! 

If you get done with this step and your classmates are still working, go back to editing the `hello.html` file in the HTML Editor and try to make **the ugliest webpage you possibly can** (you can change the appearance of text using various buttons along the top row - ex. color, bold, etc.). Send your ugly webpage contestant to the `#in-class` Slack channel.
