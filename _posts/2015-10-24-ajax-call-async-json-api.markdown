---
layout: post
title:  "Ajax Call Json API with Async False"
date:   2015-10-24 14:24:58 +0800
remark: Javascript
author: Andrew Wu
comments: true
categories: javascript
---

I only started to learn development, like seriously, when I started my first job as a developer. And honestly, before that 
I never thought one day I would be typing these out:)

As a newbie, async-ajax call is the first thing I learned completely on my own when developing a module for my company. 
It was a simple module actually, I just needed to call an ajax to get the data from SQL and interpret into JSON format and then 
proceed the action with that JSON data. But all my ajax experience till then was limited to simply loading a returned html 
element, and this is what makes the learning of this async-ajax call JSON API very unforgettable.  
 
Back to the topic, to get it done at that time, I searched online quite a bit about JSON, about how to interpret the SQL data 
into JSON format. Luckily, I found a way to create JSON object and insert the SQL data to the corresponding JSON properties. 
But then, there was another issue, which was that I need to load the data first before I use it somewhere else. And we all 
know by default, the ajax call is async, which means before it finishes,  the subsequent javascript will be implemented. 
However, without that returned JSON data, the next action I needed to implement was totally a fail. 

And I researched, researched and researched, until I found a simple way to solve the issue which was adding `Async: false` 
in that jQuery ajax call. It saved me indeed, it stopped all other javascript being implemented at the same time, meaning 
that everything else will wait until that ajax call return the json data. It helped, and I managed to finish my work. 

I know it was probably a easy one for most of you, but somehow it inspired a newbie to keep digging and keep learning. 
And maybe this is the only way how a newbie turns pro.





