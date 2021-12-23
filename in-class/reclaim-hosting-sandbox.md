---
layout: page
title: Creating a "Sandbox" on Reclaim Hosting
---

## Explore File Manager and `public_html`

Log into your Reclaim Hosting account click on cPanel. This is the overview page where you can manage a bunch of different aspects of your server account with Reclaim Hosting (such as URL domain names, setting up an email account based on your domain, etc.). Find `File Manager`and open this in a new browser tab, which will bring you to an interface showing you some folders. Much like your physical computer, your server space at Reclaim Hosting is organized into a collection of folder containing data, scripts, etc. Don't worry about what all of them mean. For now, navigate to `public_html`. This is the public-facing root folder of your server space. Basically you are going to add stuff in here (files, webpages, etc.) that you want to be accessible to other people through an internet browser.

## Make a Sandbox Directory

Your goal is to make a "sandbox" folder in your `public_html` directory that is going to be your space to install and learn new tools. This is where you can mess around and try things out. The `sandbox` folder is going to set up a structure of material that can be accessed in the following way: `https://yourdomainnameurl/sandbox/`. When you start adding sub-folders or material within your `sandbox` folder they will be just be appended to that URL 

To create your sandbox:
- Make sure you are in the `public_html` folder
- Add a new folder within your `public_html` folder called `sandbox` (make sure it says `public_html` under "New folder will be created in:")
- Navigate to the folder. It should be empty!

## Add a file to your sandbox

Now let's try adding a file into your `sandbox` folder. While still in File Manager, click +File, then name it `hello.html`. The `.html` ending tells File Manager what kind of file it is (in this case, an HTML webpage). Make sure it is being created inside your sandbox folder, then click Create New File. You should see a new file inside your directory. Select it by clicking once, then click on HTML Editor towards the top of File Manager. Click the Edit button that appears in a pop-up, and you should be seeing a blank screen with some buttons at the top. Try writing a short message here, then click the Save button. 

In a new browser tab, navigate to: `https://yourdomainnameurl/sandbox/hello.html` and you should see your message. Congratulations! 

If you get done with this step before your group members, go back to the HTML Editor and try to make the ugliest webpage you possibly can (you can change the appearance of text using various buttons) and send it to the `#in-class` Slack channel.  

## Password Protect your Sandbox Directory

Go back to cPanel under Reclaim Hosting (I recommend using a separate browser tab or using the one you left open). We are now going to add a password protection to your sandbox so that it is only viewable to people in this class (we're all going to be using the same username and password). Open Directory Privacy (under Files section), then navigate to your `sandbox` folder within `public_html`. Once in the `sandbox` folder, click Edit, then check the box for `Password protect this directory` and click Save. This will bring you to a new page, at which point you just go back one page and should see the option to type in a username and password. **Fill in the username and password provided by Professor Blevins**. This will be the same for all students so we can access each other's work. 

Have one of the members of your group try to open `https://yourdomainnameurl/sandbox/hello.html` and see if they can access it by using the same username and password. It should now be protected. 
