---
layout: post
title:      "ISP Website With Rails"
date:       2019-05-16 08:49:20 -0400
permalink:  isp_website_with_rails
---


**What is it?**

A website that allows you to buy an internet package plan. It keeps track of your payment history, service periods, and internet status changes. It connects to a router through the mtik gem and makes changes to pppoe profiles. This is a skeleton project to communicate with different routers and store information on a website. No payment API has been implemented yet.

**Features:**

* Login/Signup users
* Login users with facebook
* View all internet plans and 'purchase'
* Send router commands
* View payment histories
* View all service periods
* View all internet status changes
* Future Work

**Some features to add would be:**

* admin can look at users and their payments, service periods, and internet status changes
* admin can cancel someones service period
* admin can send commands to routers
* admin can create router profiles through the website
* automatically disconnect users with expired service periods links
* Feel free to add suggestions on my github :)!

**My Thoughts On Rails **

Rails is a very powerful framework for ruby. It has a very marked learning curve. At first, it is difficult to use. You have to stick to a lot of naming conventions that doesn't leave room for errors. Anything named incorrectly can and will cause problems. With that being said, once you get the hang of it it speeds development process by a lot. There is just too much that Rails does for you and helps you do under the covers. It handles the repetitive work so you can only focus on what makes your project unique. 

**My Experience**

For this project, I had access to some network equipment (access points, router switch, etc). I decided to try to use it as a challenge to myself and keep things interesting. I had never worked with any network equipment before, so I went to a friend of mine that helped me setup the hardware part. It took a quite a while just to be able to message the router switch with code, much more to make it do what we wanted it to do.  

 There isn't a lot of examples or documentation on the subject of router communications with ruby. The idea here is to provide a skeleton to help out other developers with similar problems. A basic router command is to change the pppoe profile of a user, so I made it around that. It can and should be modified to meet the specific needs.

 Making code that interacts with hardware components is a different experience.  The API's usually aren't very friendly and it requires you to have previous knowledge on the hardware. It is challenging but at the same time rewarding. It is fun to click a few things and watch some changes happen around you in real life. 



