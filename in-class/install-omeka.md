---
layout: page
title: Install Omeka Classic
---

## Make an Empty Directory

You are going to install an Omeka site that will be hosted with your account at Reclaim Hosting. First, we're going to create a new sub-directory in our Reclaim Hosting database where the Omeka site is going to live.

To create your sandbox:
- Log in to Reclaim Hosting with the account you created
- Go to `File Manager` and make sure you are in the `public_html` folder
- Navigate to your `sandbox` folder.
- Create a new folder inside the `sandbox` folder called `omeka`.
- If you had installed privacy settings on the `sandbox` folder for an earlier week with a username and password, go back and remove these as sometimes this can mess up the installation.

## Install and Set Up Omeka

Navigate to your cPanel in your Reclaim Hosting account. Install Omeka within your specific sub-folder you created. Instructions: <https://community.reclaimhosting.com/t/installing-omeka-classic-on-reclaim-hosting/193>

**Note: choose a username and password that you can remember** and copy/paste it somewhere for your reference. This is what you're going to use to log in to this Omeka dashboard moving forward. This is similar to Wordpress, in that you will be logging into this separately from your Reclaim Hosting account. Additionally, change the Title from "My cms" to "Omeka Sandbox"

Under My Applications in Reclaim Hosting, you should now see an Omeka installation listed along with your Wordpress installation(s). Now you should have an Omeka installation under `http://yourdomainname/sandbox/omeka`. If you go back to Reclaim Hosting's `File Manager` and go back to `sandbox` folder, open up `omeka`. If you look inside here, you will see a bunch of new folders and files that were automatically generated to "build" your Omeka site. 

Much like your Wordpress installation, in order to actually start using Omeka you need to log in to the Omeka dashboard (separate from Reclaim Hosting). The login page will be: `http://yourdomainname/sandbox/omeka/admin` , and you will use the username and password you specified when you installed Omeka. Make sure you can login before the start of class!

Before we begin, we need to change a technical setting to allow Omeka to function normally. Scroll down to the instructions on this page to configure Image Magick: <https://community.reclaimhosting.com/t/working-with-omeka-classic/194>.




