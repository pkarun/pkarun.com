---
title: 'How to Recover Site from WayBack Machine Easily'
date: Sat, 25 Jun 2016 08:33:27 +0000
draft: false
tags: ['How To', 'how to']
slug: "how-to-recover-site-form-wayback-machine-easily"
---

Recently I was buying some expired domains to build my own PBN (Private Blog Network). You might be knowing that, before buying we have to do proper domain analysis. I Have some set of criteria which I always look for before I grab those domains.

One such criteria I see is, Content on that domain. For seeing content I mainly use [http://archive.org/web/](https://archive.org/web/ "http://archive.org/web/") and sometimes I use Google Cache.

Most of the times what I do is, I just setup the domain with the existing content which I found on WayBack Machine.

There are many tools, software and services which are offering recovering service using wayback machine. If you don’t have enough time or if you don’t want to go with all these technical setup (minimal) then you can use Fiverr.com to get the things done.

​Before we start recovery process, I assume that you will be aware of below few things.

*   You know How to use SSH 
*   Comfortable with Linux Server
*   Knowledge on Domain setup process

**Requirements:**

1\. I will be using [Digital Ocean Server](https://m.do.co/c/9ab8642c13af) LAMP setup

​2. [Wayback Machine Downloader](https://github.com/hartator/wayback-machine-downloader) by Hartator

NOTE: I Recommend you to try on Fresh Server Setup if you don't know what you are doing!

Get Free $200 Digital Ocean Credit
----------------------------------

Signup with the below link and get free $200 credit on you digital ocean account. 

[Signup to Digital Ocean](https://m.do.co/c/9ab8642c13af)


Instruction on how to Download Wayback Machine Content using WayBack Machine Downloader
---------------------------------------------------------------------------------------

1\. First launch new LAMP Droplet on Digital Ocean or you can use any of your existing Linux server

2\. ​Open SSH Connection 

3\. ​Now try to install Wayback Machine Downloader on your Linux server with below command 

```gem install wayback\_machine\_downloader```

In most cases you will get below error. Because, we need Ruby to run this software.

```
root@lamp-512mb-blr1-01:~# gem install wayback_machine_downloaderThe program 'gem' can be found in the following packages:* ruby* rubygemsTry: apt-get install
```

If you got the above error, then just execute the below command to install ruby on your Linux machine.

```root@lamp-512mb-blr1-01:~# apt-get install ruby```

4\. Now we are ready to download any site fully from wayback archive easily. 

5\. ​To download site from wayback archive using Wayback Machine Downloader, we need to run the below command. Make sure it contains http:// and you replace domain.com with the domain you need to download from wayback machine.

```wayback\_machine\_downloader http://domain.com```

If you are planning to download particular time archive, then you have to use the below command.

``` wayback\_machine\_downloader http://domain.com --timestamp 20060715122318 ```

That last ID is a time which you can easily get it from wayback url. You can see the example URL below.

```http://web.archive.org/web/20060715122318/http://www.domain.com/​```

6\. Once you done with the download, you use dir command to see the directories on PWD (Present Working Directory). You will see Websites directory. Inside that you will see domain.com folder. In the folder you will see all the files related to that particular domain. 

![wayback machine downloaded folders](/how-to-recover-site-form-wayback-machine-easily/images/wayback-machine-downloader-free.png)

Once you download the folder, go and explore the folders and files. Now you go to new domain setup and place those folders and files in the same directory structure. 

I hope this small tutorial is helpful for you guys. 

If you have any doubts related to this tutorial, feel free to ask on comments.