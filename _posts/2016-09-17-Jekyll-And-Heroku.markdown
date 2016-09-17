---
layout: post
title:  "Jekyll And Heroku"
date:   2016-09-17 14:05:00 -0400
categories: hosting
---


Over the past 2 days I have been working to setup this website > www.jordantomasone.com, the website itself runs on Jekyll static webpage generator developed by github. Originally I had planned to use github pages to host the site but I encountered some issues because I create the git repo under its own organization, and by doing so, would of had to use www.jordantomasone.com/app-name (with app-name being the name of the app), this was a little messy for my liking so I decided instead of creating a brand new github account and hosting it on github pages I would try another option.

So while I weighed my options I remember that my AWS only has 3 months left on the free 12 month period so as well instead of creating a new account or using it for 3 months and switching I kept looking, this was my mistake.

I ended up find Heroku as an option, there cloud services for ruby deployment is really praised thoughout my research so I decided to take the plunge and check it out. So Heroku itself is not a bad option at all its just for using a static webpage generator it kind of loses its purpose, unlike github pages Heroku needs to precompile all page assets or it basically just interperts static pages. So in the end uploading the _site/ folder is all that is need.

So what I have learned is that using Heroku with Jekyll is pointless, github pages and AWS are always better alternatives, but don't take my word for it try it yourself.

J
