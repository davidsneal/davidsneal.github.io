---
layout: post
title: Transferring files from one server to another
excerpt: This is an excerpt
---

This article is about my personal favourite Linux/UNIX command `scp`, including a brief example of how it can be used.

-----

### SCP

Having had to migrate a large number of sites to new servers recently, finding this command was a real lifesaver. My knowledge has grown considerably over the years and having to perform tasks like this sent me on the quest to find the ideal solution.

**Back in the day...** I used to do everything via FTP, by downloading all the files locally before uploading them to the new destination. This could take forever, and waiting for each file to tick by was a painful process.

**A little while later...** After beginning to get used to a few simple shell prompts, I heard it was possible to compress folders in a single command, so I was keen to give this a go. Problem was when things need to be done quickly, I had to weigh up the time it would take to learn how to do this over simply doing it by FTP. Getting it done using FTP won for a while but in the end I took the time on my own development server and found it was a doddle.

Compress all files: `tar -zcvf compressed_website.tar.gz /var/www/website`

Then after downloading this archive and uploading it to its new location, you simply run `tar -zxvf compressed_website.tar.gz -C /var/www/newwebsite`

 > I hope it goes without saying that have to amend directories as required!
 
**A couple of years later...** Admittedly it perhaps should have been sooner, but it wasn't until I needed to upgrade to a new server that I clicked it may possible... I suddenly thought - '*Maybe there is a way to transfer files directly from one server to another*'.

Much to my delight, there is!

There are a number of other options available, but to transfer a whole directory recursively (*it and all its contents*), simply run `scp -r dirtomove/ user@destip.com:/dest/dir/`

Enter in the user's password and **job done!** Just watch the files transfer over.