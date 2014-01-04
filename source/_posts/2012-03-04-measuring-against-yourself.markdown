---
layout: post
title: "Measuring against yourself"
date: 2012-03-04 21:39:27 +0100
comments: true
categories:
---
Hackers often obsess about how to write great code - code that is readable, performs well, is easy to maintain or meets other specific expectations. If you get a group of hackers in a room and it so happens that this is not the topic of their discussion then they most likely talk about productivity - about how to build software quickly and efficiently, how to type fast, which development environment to choose, which programming language makes them more productive, etc.
<!-- more -->
<img style="float: left; margin: 0px 15px 15px 0px;" src="/images/road_to_nowhere.jpg" />

This is really great. That’s what hackers are supposed to do. It’s a tremendously important aspect of the art of creating software. Sometimes it really does boil down to how fast you can get the job done. What surprisingly few of us realize is that the single most inefficient thing to do is to write code that brings no value to your project.

I’ve seen it happen over and over again. You set out to build something only to realize that hardly anybody is ever using it or that it has no effect on your users. Sure, it’s there and it works but it doesn’t **DO** anything that your users actually need. In those cases you may as well write:
{% gist 2165107 %}
It will accomplish pretty much the same and it doesn’t really get more readable and efficient than that.
Productivity is a pretty peculiar thing. You may be working like crazy - write lines after lines of code and yet accomplish absolutely nothing. In startups, when the team is small and time is always short, it can literally mean the life and death of the company. Deciding what to code is among the most important decisions you have to make. Period.

Building stuff for the sake of the activity alone may be fun but it doesn’t get you very far in business. It kills you. But how do you know if whatever you’re building gets you closer to your goal? Well, there’s an old management adage that goes like this:
{% blockquote %}
You Can't Manage What You Don't Measure
{% endblockquote %}
How do you measure whether your new, shiny feature gives you better user retention, increases your conversion rates or achieves any other goal you’ve set out to achieve with it? Sure, it’s fairly easy to measure if your users are using it but it still doesn’t tell you what its impact is on set goals. The problem is that when you see a change in your metrics, you don’t really know what caused it. It could be the recently introduced feature, but it could as well be the article on [TechCrunch](techcrunch.com) that ran 2 months prior and incidentally turned into a flamewar on [reddit](reddit.com) a day before. The problem is that you can never test things in complete isolation.

So are we completely doomed to imagine things and guess what will work and how?
That’s what I thought until I read [Freakonomics][freak] some years ago. It turns out that there is a class of problems that are seemingly immeasurable but in fact can be measured with high degree of probability. Here’s an excerpt from the book:

{% blockquote [Steven D. Levitt and Stephen J. Dubner http://www.amazon.com/s/?_encoding=UTF8&camp=1789&creative=390957&field-keywords=freakonomics&linkCode=ur2&sprefix=freakono%2Caps%2C283&tag=nedzynski-20&url=search-alias%3Daps Freakonomics] %}
Of all the truisms about politics, one is held to be truer than the rest: money buys elections. (...) Indeed, election data show it is true that the candidate who spends more money in a campaign usually wins. But is money the cause of the victory? (...) Picture two candidates, one intrinsically appealing and the other not so. The appealing candidate raises much more money and wins easily. But was it the money that won him the votes, or was it his appeal that won the votes and the money? That’s a crucial question but a very hard one to answer. Voter appeal, after all, isn’t easy to quantify. How can it be measured?

It can’t, really—except in one special case. The key is to measure a candidate against… himself. That is, Candidate A today is likely to be similar to Candidate A two or four years hence. The same could be said for Candidate B. If only Candidate A ran against Candidate B in two consecutive elections but in each case spent different amounts of money. Then, with the candidates’ appeal more or less constant, we could measure the money’s impact. (...)

Here’s the surprise: the amount of money spent by the candidates hardly matters at all. A winning candidate can cut his spending in half and lose only 1% of the vote. Meanwhile, a losing candidate who doubles his spending can expect to shift the vote in his favor by only that same 1%. (...) Some politicians are inherently attractive to voters and others simply aren’t, and no amount of money can do much about it.
{% endblockquote %}

This short example really opened up a few doors in my head. To this day I find the concept of measuring something in relation to the same thing in different circumstances to be pretty cool. The idea of A/B testing has been around for quite some time but I wasn’t sure how to apply this to software development for quite a while...
{% pullquote %}
So how does this approach translate into our decision-making process regarding which features to cut and which ones to double down on?

It turns out that all it takes is having the capability to deploy a particular functionality to a select group of your users and to measure the impact of the change in comparison to similar reference group without that feature. {" It’s a pretty simple concept and yet in many cases this approach can make all the difference. "} This way you could clearly determine that for example: 'displaying cute kitten images on logout' makes your users 5% more likely to convert to paying customers within a week. Pretty neat, right?
{% endpullquote %}

This is why I love [Lean Startup][lean] so much. It is essentially a framework that gives you a clear formula on how to build your product and your business based on the idea of comparative measurement. Yes, it’s quite an overhead to build the framework for partial deployments, for gathering user data and computing metrics but without it you’re blind - you’re just playing a guesswork game. Can your business afford it?

[freak]: http://www.amazon.com/s/?_encoding=UTF8&camp=1789&creative=390957&field-keywords=freakonomics&linkCode=ur2&sprefix=freakono%2Caps%2C283&tag=nedzynski-20&url=search-alias%3Daps Freakonomics
[lean]: http://www.google.com/url?q=http%3A%2F%2Fwww.amazon.com%2Fgp%2Fproduct%2F0307887898%2Fref%3Das_li_qf_sp_asin_il_tl%3Fie%3DUTF8%26tag%3Dnedzynski-20%26linkCode%3Das2%26camp%3D1789%26creative%3D9325%26creativeASIN%3D0307887898&sa=D&sntz=1&usg=AFQjCNGou3F72ifIdMzfPalUN_0vAv824A Lean Startup