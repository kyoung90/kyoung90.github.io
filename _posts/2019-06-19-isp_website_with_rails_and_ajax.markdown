---
layout: post
title:      "ISP Website With Rails And AJAX"
date:       2019-06-19 23:50:09 -0400
permalink:  isp_website_with_rails_and_ajax
---


**What is it?**

A website that allows you to buy an internet package plan. It keeps track of your payment history, service periods, and internet status changes. It connects to a router through the mtik gem and makes changes to pppoe profiles. It has http routes for giving out data in JSON format, and it uses it to display some content without having to refresh. This is a skeleton project to communicate with different routers and store information on a website. No payment API has been implemented yet.

**Features:**

* Login/Signup users
* Login users with facebook
* View all internet plans 
* 'Purchase' internet package services and show receipt without having to refresh the page
* Navigate through internet packages without having to refresh the page
* Send router commands
* View payment histories
* View all service periods
* View all internet status changes
* Admins can view all users that have active service period for a particular internet package

**Some features to add would be:**

* Make all index pages work asynchronously
* Admin can cancel someones service period
* Admin can send commands to routers
* Admin can create router profiles through the website
* Automatically disconnect users with expired service periods links**

Feel free to add suggestions on my github :)!

**My experience:**

This project was different from others. I had to build on an existing rails project instead of building one from scratch. The main challenge was building your own API (displaying JSON data through http routes). Then, using that data, display content on the website.  

I gotta say, learning how to use AJAX makes a ton of difference. The end result feels more smooth, and more production like. Having that knowledge on how to build your own API gives you another level of understanding of code.  It helps deal with impostor syndrome. 

API's no longer feel as magical once you know how to do them yourself. How easy it is to do with rails is ridiculous (in a great way!). The strange part about AJAX is having to mix up Javascript, HTML, and CSS, all from different files. The code gets clunky. This is where react could make a difference. It could help by making reusable components with their own logic all together. That would solve the main issues about just using jQuery and rails.

I can't wait to mix this up with react. It feels like it is the next step to becoming a developer in today's world. It is one of the main components that empower you to feel confident building projects.
