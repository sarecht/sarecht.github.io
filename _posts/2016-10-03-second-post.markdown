---
layout: post
title:  "Cybersecurity Club"
date:   2016-10-04
categories: community
author: "Sarah Albrecht"
---

I joined UNC's Cybersecurity Club and it's going exactly how I thought it would:
I'm very confused and the other members are very good with computers already.

For the first hands on activity, we made accounts on 
<a href=" ">https://www.hackthissite.org/</a>. This site provides users with 
fake tasks to complete in order to test and establish "hacking" skills when it
comes to cybersecurity. 

The first task we did was a beginner "real life" task where we were supposed to
find the secret log in page for a white supremist group's website so we could
ruin their method of communication. This involved looking at the HTML of the 
website and finding a secret element that showed up in the HTML, but not on the 
page itself. I was able to nagivagate through the HTML pretty well and 
understand what everything meant. Someone else in my group solved this part first
and we moved on to the next step, which was the hardest part. We had to find a 
way to log in as a member without actually having a username or password for the
website. It didn't just involve guessing, either: the goal was to trick the 
website into thinking whatever you wrote was valid as a username and password.

What I learned is that to do this you need to use a SQL Injection Attack. I had
no idea what SQL was before I went to this meeting. I learned that it's a 
programming language for managing databases. In order to log in to the fake 
website, you needed to type 

{% highlight html %}
' or 1=1--
{% endhighlight %}

into both the username and password fields. A lot of this information is still
over my head, but from what I understand you are giving the database an 
expression that is always true instead of a username or password. Doing this
allows you to log in to the website.

I found learning this to be very interesting because I had no idea that it was
possible to trick a website in this way. During this meeting we discussed
how most companies and websites have a way to prevent people from doing this by
writing a more secure code. 

Overall, participating in this simulation taught me more about how important
html is to understanding a webpage and gave me my first experience with
cybersecurity. I never would've completed this simulation on my own, but I hope
that as I work through more simulations on HackThisSite and work with html more in
INLS 161 I can understand these concepts more and learn to solve problems on my
own.
