---
layout: post
title: GitHub Pages and Jekyll
excerpt: This is an excerpt
---

Considering this blog itself is powered by [Jekyll](http://jekyllrb.com) and powered by [GitHub](https://github.com/), it seems quite fitting that my first post should be about it.

-----

### GitHub Pages

As if GitHub doesn't do enough for the developer community with its free Git repository functionality, you can also **host a website with them for free!** No, I'm not joking, you can even use a custom domain.

If you want to go ahead and get started the first thing you need to do is create a new repository. It must be named **username.github.io**. 'username' must be replaced with your GitHub username in order for it to work, such as [davidsneal.github.io](https://github.com/davidsneal/davidsneal.github.io).

Clone your new repo locally, add some content and push it back up to the master branch. It'll take a couple of minutes for the site to show up. Once your site is up and running, you'll be impressed with the speed as you shall automatically be taking advantage of GitHub's Content Delivery Network.

Check out the latest information regarding GitHub pages [here](https://pages.github.com/).

-----

### Jekyll

Simply put...
 > Jekyll takes plain text post files and transforms them into blog posts, such as the one you're reading now.

There a heck of a lot more to it than that, but that's the main essence I have picked up over my short experience with it, dramatically condensed into a single sentence.

I've not got too far through the [Jekyll documentation](http://jekyllrb.com/docs/home/) yet, but it seems very comprehensive and well explained. Serious kudos for the design of their site too.

Installation took me a little longer than was made out, but **Ruby** is still completely alien to me. I got held up on the very first step `gem install jekyll`, receiving a message it appears many others have seen too:

 > You don't have write permissions for the /Library/Ruby/Gems/2.0.0 directory.
 
After a visit to stack**overflow** I installed [Ruby Versions Manager](https://rvm.io/), before returning to stack**overflow**. Once I'd got that sorted Jekyll was a breeze to get running, and I had the base install site up and running in under a minute.

There are some great Jekyll themes out there, for anyone wondering, this theme is called [Hyde](https://github.com/poole/hyde).