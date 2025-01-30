---
title: 'How to Integrate GrooveFunnels with Sendy'
date: Tue, 15 Sep 2020 19:19:24 +0000
draft: false
tags: ['email marketing', 'GrooveFunnels', 'How To', 'how to']
slug: "groovefunnels-integration-with-sendy"
---

If you are using [GrooveFunnels](https://groovepages.groovesell.com/a/yy7tlmP3Kxgu) and looking to integrate your GrooveFunnels/GroovePages with sendy.co email marketing platform, then you are in the right place.

In this article, you will learn how easily we can use sendy with groovefunnels without using zapier.

Currently, groovefunnels are not offering any inbuilt solution to integrate sendy with groovepages, so we need to use some other solution.

In this post, I'm going to show you how you can use a sendy API to integrate with the groove platform.

How to Integrate Sendy with GroovePages/GrooveFunnels:
------------------------------------------------------

### Step 1: Download Sendy Code

To integrate your sendy email platform with the groove platform, you first need to download the code file. Download the sendy code from the below link (using real GrooveFunnel landing page with Sendy.co optin Integration).

[Download Sendy Code Here](https://drive.google.com/uc?export=download&id=1sk-taIiCk-fZs9sDH3FIXPSt_i5w-get)

### Step 2: Configure Your Sendy Code

For each new list on sendy, you need to configure the sendy code file.

You need to update the Sendy installation URL, Sendy list ID, Sendy API Key, Success page URL, and Fail page URL on the code file which you have received.

```
 //-------------------------- You need to set these --------------------------//
	$your_installation_url = 'https://sendyinstalleddomain.com/'; //Your Sendy installation (without the trailing slash)
	$list = 'Ysd6Zy1Yus8JSfV7639GKAfA'; //Can be retrieved from "View all lists" page
	$api_key = '2pM9pTFlqRpICQOWTBNP'; //Can be retrieved from your Sendy's main settings
	$success_url = 'https://pkarun.com/thank-you/'; //URL user will be redirected to if successfully subscribed
	$fail_url = 'https://pkarun.com/contact-us/'; //URL user will be redirected to if subscribing fails
	//---------------------------------------------------------------------------//
```

### Step 3: Upload Configured Sendy Code to Your Server

Once sendy code configuration is done, now it's time to upload the code file to your server.

I uploaded that file to the sendy folder itself. I prefer the below file structure for easy to remember purpose.

```
https://sendydomain.com/groovefunnels/pkarun.com/sendy-code-optin.php
```

### Step 4: Link Your Groovefunnel Optin with Sendy Code

![](/groovefunnels-integration-with-sendy/images/groovefunnels-sendy-integration-1024x406.png)

Now go to **Blocks** \=> **Forms**, and grab any optin form.

![](/groovefunnels-integration-with-sendy/images/sendy-groove-pages-1024x497.png)

Now select the email input field and make sure you selected the "**input**" field by having a look at the bottom navigation bar, and in **Input name,** make sure it is "**email**" and check other settings as shown in the above image and hit **Update** option.

![](/groovefunnels-integration-with-sendy/images/sendy-groovefunnel-email-optin-1024x525.png)

Now it's time to configure groove optin form.

To configure groove optin form, select **complete optin form** and confirm by having a look at bottom navigation bar. It should show "**form-container**".

On right panel you will see form-container configuration box is open. Click on "**Configure**" and under **Form action** choose **POST** and for **Form POST URL** put your **sendy configuration .php file path** and hit **Update** and **Publish** the site.

**Note**: If you don't publish site you cannot able to test optin form so make sure you publish the page before testing.

That's it.

Now go and test your groovefunnels and sendy.co integration. It should work.