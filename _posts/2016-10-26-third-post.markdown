---
layout: post
title:  "Assignment 3 Review"
date:   2016-10-26
categories: assignments
author: "Sarah Albrecht"
---

![alt text](http://s2.quickmeme.com/img/4c/4c7b211bcd281a8f2e6c26b144c951a50d69a0046f0ef117ee330ceb6279c712.jpg "scripting meme")



For assignment 3, I chose to work with part of a paper I had to write for my
ENGL 105 class last year. We had to do a report on a controversial drug of our
choice and then write about whether or not we believed it should be used. I chose
Prolixin, which is an antipsychotic used in treating schizophrenia. Like many
antipsychotics, it can have severe side effects on the user and in this paper
I briefly introduce the drug and explain its side effects.

My paper was saved on Google Drive for some reason, so I downloaded it as a 
Microsoft Word document, which i learned is a docx file. I then uploaded it to my
Cloud9 workspace and converted it to a markdown file using the command:

{% highlight html %}
pandoc --smart -o prolixin.md prolixin.docx
{% endhighlight html %}

From here I created a script that converts the markdown file to html, odt, pdf, 
and docx. This was a lot of copying and pasting and then changing the file types.
The files in my folder now are:


[prolixin.odt](https://github.com/sarecht/assignment-3-sarecht/blob/master/prolixin.odt)
    
[prolixin.pdf](https://github.com/sarecht/assignment-3-sarecht/blob/master/prolixin.pdf)
    
[prolixin.docx](https://github.com/sarecht/assignment-3-sarecht/blob/master/prolixin.docx)
    
[prolixin.html](https://github.com/sarecht/assignment-3-sarecht/blob/master/prolixin.html)

After I did this, I tweaked my script to say the current date and time and
some friendly dialogue.

One of the challenges I faced completing this assignment was with the image
I chose to use. The first challenge was enabling Cloud9 to find my photo by
uploading it to the workspace. After this my picture showed up, but it was consistently
in the wrong place. I decided to search for a way to use page breaks in markdown, but
it wasn't working, and it wasn't until Elliot said to search specifically for pandoc
that I found the right way to do it. This seems pretty obvious looking back, but 
I guess these things slip your mind sometimes when there's so  much else going on
in a project.
Another challenge I faced was figuring out smart quotes because I knew what they
are but I had issues implementing them. In the end I added the `--smart` operator
to retain the smart quotes when converting the file, so I'm hoping that worked
out in the end. 

Overall I thought this project was really interesting because until recently
I thought that Microsoft Word was the most useful program for writing documents.
When I was working with my document on word, though, I noticed how annoying it was
to try to rearrange my photos and format my document properly. When I opened the markdown
file of the same document I noticed how much easier it was to work on it that way. 
Hopefully in the future I can avoid any Microsoft Word headaches using what I learned
in this assignment.

[My script](https://github.com/sarecht/assignment-3-sarecht/blob/master/sarecht-convert-docs.sh)

[Editor](https://ide.c9.io/sarecht/assignment-3)